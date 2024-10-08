[![example-shiny-python](https://github.com/koyeb/example-shiny-python/actions/workflows/deploy.yaml/badge.svg)](https://github.com/koyeb/example-shiny-python/actions)

<div align="center">
  <a href="https://koyeb.com">
    <img src="https://www.koyeb.com/static/images/icons/koyeb.svg" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">Koyeb Serverless Platform</h3>
  <p align="center">
    Deploy a Shiny application in Python on Koyeb
    <br />
    <a href="https://koyeb.com">Learn more about Koyeb</a>
    ·
    <a href="https://koyeb.com/docs">Explore the documentation</a>
    ·
    <a href="https://koyeb.com/tutorials">Discover our tutorials</a>
  </p>
</div>


## About Koyeb and the Shiny Python example application

Koyeb is a developer-friendly serverless platform to deploy apps globally. No-ops, servers, or infrastructure management.  This repository contains a Shiny application written in Python that you can deploy on Koyeb in a single click.

This example application is designed to show how web application built with Shiny for Python can be built and deployed on Koyeb.  The application is created from the [Shiny map distance template](https://shiny.posit.co/py/templates/map-distance/), allowing you to deploy an interactive, data-driven application to demonstrate Shiny functionality.

## Getting Started

Follow the steps below to deploy and run the Shiny for Python application on your Koyeb account.

### Requirements

You need a Koyeb account to successfully deploy and run this application. If you don't already have an account, you can sign-up for free [here](https://app.koyeb.com/auth/signup).

### Deploy using the Koyeb button

The fastest way to deploy the Shiny for Python application is to click the **Deploy to Koyeb** button below.

[![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=shiny-python&type=git&repository=koyeb%2Fexample-shiny-python&branch=main&builder=buildpack&run_command=shiny+run+--host+0.0.0.0+--port+8000+app.py&instance_type=micro&env%5B%5D=&ports=8000%3Bhttp%3B%2F)

Clicking on this button brings you to the Koyeb App creation page with everything pre-set to launch this application.

_To modify this application example, you will need to fork this repository. Checkout the [fork and deploy](#fork-and-deploy-to-koyeb) instructions._

## Fork and deploy to Koyeb

If you want to customize and enhance this application, you need to fork this repository.

If you used the **Deploy to Koyeb** button, you can simply link your service to your forked repository to be able to push changes.  Alternatively, you can manually create the application as described below.

On the [Koyeb Control Panel](https://app.koyeb.com/), on the **Overview** tab, click the **Create Web Service** button to begin.

1. Select **GitHub** as the deployment method.
2. In the repositories list, select the repository you just forked.
3. Select your preferred region and Instance type.
4. Open the **Builder** section.  Click the **Override** toggle associated with the **Run command** and enter `shiny run --host 0.0.0.0 --port 8000 app.py` in the field.
6. Choose a name for your Service, i.e `shiny-python`, and click **Deploy**.

You will be taken to the deployment page where you can follow the build of your Shiny for Python application. Once the build is completed, your application will be deployed and you will be able to access it via `<YOUR_APP_NAME>-<YOUR_ORG_NAME>.koyeb.app`.

## Contributing

If you have any questions, ideas or suggestions regarding this application sample, feel free to open an [issue](https://github.com/koyeb/example-shiny-python/issues) or fork this repository and open a [pull request](https://github.com/koyeb/example-shiny-python/pulls).

## Contact

[Koyeb](https://www.koyeb.com) - [@gokoyeb](https://twitter.com/gokoyeb) - [Slack](http://slack.koyeb.com/)
