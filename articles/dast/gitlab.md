# How to Integrate SOOS DAST with your GitLab CI

<img src="/assets/img/SOOS-Icon.png" alt="SOOS" width="128" height="128">
<img src="/assets/img/gitlab/gitlab.png" alt="GitLab" width="128" height="128">


This document will take you step-by-step through the tasks required to set up a GitLab repo, for scan it with the SOOS DAST Product.

## Prerequisites
- You need to have a SOOS Account.
- You need to have a GitLab repo.

## Steps

### Configure the `Client Id` and the `API Key` values <!-- Shared content -->
To be able to run a `SOOS DAST Analysis Scan` you need to get the `Client Id` and the `API Key` from the SOOS Application.
<!-- Add screenshot of place where you can get it -->
1. Go to [SOOS](https://app.soos.io) and log into it using your `SOOS` account.
2. In the menu on the left side of the screen, click on `Integrate` menu option.

<img src="/assets/img/soos-menu.png" alt="SOOS Menu" height="400">

3. On the `API Credentials` section, you will see the `API Key` and the `Client Id` values. You need to copy both clicking on the copy button

<img src="/assets/img/api-credentials.png" alt="API Credentials section">

**Note**: We strongly recommend using a `Service Account` for integrations. Read more about `Service Accounts` and how to create them [here](https://kb.soos.io/help/what-is-a-service-account-user-and-when-might-i-need-to-create-one). 

4. Go to your `GitLab` project and navigate to the `CI/CD Settings`

<img src="/assets/img/gitlab/settings.png" alt="GitLab Settings">

5. Press the `Expand` button within the `Variables` section:

<img src="/assets/img/gitlab/variables.png" alt="GitLab Variables">

6. Create the `SOOS_API_KEY` and `SOOS_CLIENT_ID` variables using the values copied on step 3. These will serve as environment variables to be used by the `SOOS DAST Scan Analysis`.

### Create or Update your `.gitlab-ci.yml` file

Once the `SOOS_CLIENT_ID` and `SOOS_API_KEY` have been configured, the next step is create or update the `.gitlab.yml` file.

**Note:** You need to create a `.gitlab-ci.yml` file in your repository root directory if you don't have it.

1. Copy the content below in your `.gitlab-ci.yml` file to run the `SOOS DAST Analysis`:

<script async type="text/javascript" src="https://gist.github.com/soostech/7b74eb66cc1bde6cc4506eb67538fc14.js"></script>





