# Hahn.ApplicatonProcess.May2020
.Net Core 3.1 with Aurelia 

## Tools
Microsft Visual Studio 2019
.Net Core 3.1, .Net Standard 2.1.
NPM v6.4.1
Node v10.15.3

## Building

Download [Zip](https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020)

Extract Hahn.ApplicatonProcess.Application.zip.
1. Open Solution from extracted folder "Hahn.ApplicatonProcess.Application.sln" in Microsft Visual Studio 2019
2. Make sure "Hahn.ApplicatonProcess.May2020.Web" is selected as Startup Project
	<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/SolutionSetup.JPG" width="800" />
3. Just press F5 to build(including npm) and run the application

Note: npm is configured in project file

If you want to run npm, navigate into "Hahn.ApplicatonProcess.Application\Hahn.ApplicatonProcess.May2020.Web"

//for development build
Run> npm run build:dev 

//for production build
Run> npm run build 

##Screens Overview

1. Home page will appear like below (red highlighted are options)
<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/Home.jpg" width="900" />

2. New Applicant (with valid data)
<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/valid_form.JPG" width="900" />

3. New Applicant (with validation errors)
<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/not_valid.JPG" width="500" />

3. New Applicant (after language change. Place holders are not under localization yet)
<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/after-lng-change.JPG" width="500" />

4. New Applicant (Reset popup)
<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/reset.JPG" width="500" />

5. Applicant Details (after adding)
<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/view.JPG" width="500" />

6. To go to edit view from list
<img src="https://github.com/muthuesign/Hahn.ApplicatonProcess.May2020/blob/master/Docs/to-go-view.png" width="900" />

## Publishing

1. Bump the version
  
  ```shell
  npm run bump-version [<newversion> | major | minor | patch]
  ```

2. Prepare the release (run tests, run build, docs, release notes)
  
  ```shell
  npm run cut-release
  ```

## Uncompleted Task

- when the user has touched a field but afterwards deleted all entries, the reset button is also not enabled.

