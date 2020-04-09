# Task List For Project setup

You should complete these tasks throughout the day to get your project setup for development.

## Team Name
Numbers are boring -- come up with a name for your dev team!

## Gitlab
1. Create a group for your team
1. Also add @danieltunon as a member to the group
1. Add a Client Gitlab Repo to group
1. Add a Backend Gitlab Repo

## Hello World Client
Use `create-react-app` to get the client bootstrapped and connect to your repo.

## Hello World Backend
Use Spring Initialzr to get your backend bootstrapped


## Heroku
Heroku Teams unfortunately require a credit card to set up. Instead have one team member creat the app under their account (or create a team email and use it to make a heroku account) and add all team members as collaborators (the need heroku accounts too).
1. Create App for Client
    * In the app settings configure the `buildpack`: add the url  https://github.com/mars/create-react-app-buildpack
1. Heroku App for Backend
    * In the app settings configure the `buildpack`: add the url heroku/jvm
    * Add postgres db addon

## CI/CD
Use the teplates provided to get started setting up CI/CD for your projects. You can customize these if you wish. This is just a starting point. 
* The `gitlab-ci.yml` and `system.properties` files should be placed in the root of your project. 
* You can specify a different java version if you need to in `system.properties`.
* The `package.json` has updates used in the CI/CD (jest test coverage)
* The `application.yml` tells spring boot to use Heroku defined environmenmt variables  in prod to run your app
* You need to generate a Heroku API Token and add it to both the repositories' Settings > CI/CD > Variables (munu on the left of repo has `Settings`). The example `gitlab-ci.yml` files reference it as `HEROKU_API_KEY`

## TWA
Finish your TWA with team if not done. One final element that is part of the team working agreement is the schedule of the daily and weekly ceremonies. As a team decide on the time and day for each. Retro should be on Friday. I would like to be able to attend the retros if the teams are willing to accomodate this, please make sure the retros do not overlap.
1. Iteration Plannong Meeting
1. Backlog Refinement Meeting
1. Retro

Send a calendar invite for your chose time to danny.tunon@galvanize.com