# Automation-Ruby-Framework

What is this repository for?

Acceptance and regression tests
UI tests
Endpoints tests
How do I get set up?

Ruby 2.2.1 installed
Go to the project's root directory
Run bundle install
How to run the tests?

Local machine

Running rspec from command line will start running all the tests on your local machine using Firefox browser
Optional you can run rspec spec -f JUnit -o results.xml and the results will be saved in the xml file.
You can use all rspec_command_line-params
Selenium Grid

Set environment variables:
export remote=yes
export hub=grid
Optionally you can set: grid_ip and grid_port, otherwise it will use the default grid
Now run the tests as on local machine
BrowserStack local

You need browserstack local binary so you have to follow the steps from bs_local testing
Run it: ./BrowserStackLocal f7ebLDyJZPzoRfUkxcB5 -localIdentifier "BrowserStackLocal" -forcelocal localhost,3000,0
Set environment variables:
export remote=yes
export hub=browserstack
Set optional environment variables: bs_browser, bs_browser_version, bs_os, bs_os_version, bs_device using values from bs_capabilities, otherwise it will use windows 8.1 and Firefox 44.0.
Now run the tests as on local machine
Jenkins
