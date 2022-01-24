# How to Integrate SOOS DAST with your GitLab CI

<img src="/assets/img/SOOS-Icon.png" alt="SOOS" width="128" height="128">
<img src="/assets/img/gitlab/gitlab.png" alt="GitLab" width="128" height="128">


This document will take you step-by-step through the tasks required to set up a GitLab repo, for scan it with the SOOS DAST Product.

## Prerequisites
- You need to have a SOOS Account.
- You need to have a GitLab repo.

## The `Client Id` and the `API Key` values <!-- Shared content -->
To be able to run a `SOOS DAST Analysis Scan` you need to get the `Client Id` and the `API Key` from the SOOS Application.
<!-- Add screenshot of place where you can get it -->
1. Go to [SOOS](https://app.soos.io) and log into it using your `SOOS` account.
2. In the menu on the left side of the screen, click on `Integrate` menu option.

<img src="/assets/img/soos-menu.png" alt="SOOS Menu" height="400">

3. On the `API Credentials` section, you will see the `API Key` and the `Client Id` values. You need to copy both clicking on the copy button

<img src="/assets/img/api-credentials.png" alt="API Credentials section">

4. Go to your `GitLab` project


