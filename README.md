# RinRuby-Heroku-Sample
This app serves as a sample to get you started using RinRuby on heroku. 

## Getting Started
1. Fork and Clone repo
2. Create heroku instance with heroku-buildpack-multi
  * `heroku create --stack cedar-14 --buildpack https://github.com/ddollar/heroku-buildpack-multi.git`
3. Push to heroku
  * `git push heroku master`

## Details
This app uses (heroku-buildpack-multi)[https://github.com/ddollar/heroku-buildpack-multi] to run both Ruby and R in the same build. This works with the `.buildpacks` file to define the buildpacks to use. 
