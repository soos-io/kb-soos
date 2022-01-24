# How to Configure the Environment Variables
In this section, we will see how to store the `SOOS Client Id` and the `SOOS API Key` values used by the scripts (SOOS SCA and SOOS DAST) in two environment variables.

## Definitions
- `SOOS Client Id` is a unique value associated to an `organization`.
- `SOOS API Key` is a unique value associated to an `account`.

Two accounts that belongs to an organization will have the same `SOOS Client Id` value but different `SOOS API Key` values.

## Get the values from SOOS
1. Go to [SOOS](https://app.soos-io) and log into the application with your account.
2. In the menu (placed on the left side of the screen), click on `Integrate`option.
<!-- Put here a screenshot of the  menu-->
3. Copy the `SOOS Client Id` and `SOOS Api Key` values and store it temporally. Both will be needed later


## Store the SOOS Client Id and the SOOS API Key as Environment Variables.
In this section, we will create two environment variables: `SOOS_CLIENT_ID` and `SOOS_API_KEY`. The `SOOS Client Id` value will be stored on the `SOOS_CLIENT_ID` environment variable and the `SOOS API Key` value will be stored in the `SOOS_API_KEY` environment variable.
<details>
    <summary>Linux/MacOS</summary>
<p>
1. Open the `terminal` or `command console`
2. Run these commands:

``` shell
export SOOS_CLIENT_ID = 54w45w.... # Paste SOOS Client Id value copied on 
export SOOS_CLIENT_ID = 54w45w.... # Paste SOOS API Key value
```

</p>
</details>

<details>
    <summary>Windows</summary>
</details>
