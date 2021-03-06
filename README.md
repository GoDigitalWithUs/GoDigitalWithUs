#[GoDigitalWith.Us](http://www.godigitalwith.us/)
![ruby version](https://img.shields.io/badge/ruby-2.3.1-brightgreen.svg)

<center>
  ![](https://www.whitehouse.gov/profiles/forall/modules/custom/gov_whitehouse_www/images/icons/wh_logo_seal.png "White House")
</center>

#####*A web platform to help close the Digital Divide in collaboration with the White House*
---

### Table of Contents
* [What is GoDigitalWith.Us?](#what-is-godigitalwith.us?)
* [How to contribute](#how-to-contribute)
* [Getting started](#getting-started-in-osx)

---

### What is GoDigitalWith.Us?
The Obama Administration announced the [ConnectALL Initiative](http://make.sc/whitehouse) in March 2016 to give all Americans access to broadband connectivity. In order to do so, the administration called on the tech community to help the United States to move more of its population on to the Internt. A team of students at [Make School](https://www.makeschool.com/founding-class) conducted weeks of user research and designed GDWU as an open-sourced curated online repository of Internet/computer skills tutorials as a mobile-friendly responsive web-app.

A basic digital literacy suite is shipped with the app of Computer Basics and Internet Basics as a tool for those just getting started with new technologies. Content is contritubed to by the nationwide community of "tech helpers". Our tech helpers include tech labs, librarians, volunteers and anyone who can provide tutorials to help our community become better connected throughout our nation.

### How to contribute
There are several ways to contribute to the project!

* **Contribute content**: In order to be successful, we need all of you to provide content to help those understand how to connect using the Internet. Things that seem basic and intuitive to those that have grown up with technology can seem daunting to many who have never used it. Spend 30 minutes creating a tutorial and submit it for review! It can be something a simple as creating an email account with yur favorite email service!

* **Create issues**: Found a bug? Have a suggestion? Please open an [issue](https://github.com/cmaher92/ConnectAll/issues) so we can take a look!

* **Contribute to our code**: Found a fix for a bug? Want to add a feature? Create a [pull request](https://github.com/cmaher92/ConnectAll/pulls) and we'll take a look!

* **Get involved**: If you'd like to get more involved, please feel free to contact us at `godigitalwithus@gmail.com`.

### Getting started in OSX
1. Clone the project

  ```
  git clone https://github.com/cmaher92/ConnectAll.git
  ```

1. Install rbenv: If you already have Ruby and need to update to 2.3.1, skip to step 3.
  * Install Hombrew: If you have Homebrew, skip to next step.

    ```
    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    ```

  * Update Homebrew

    ```
    brew update
    ```

  * Install rbenv

    ```
    brew install rbenv
    ```

1. Install Ruby
  * Update `ruby-build`

    ```
    git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
    ```

  * Install Ruby 2.3.1

    ```
    rbenv install 2.3.1
    ```

  * Set global Ruby version to 2.3.1

    ```
    rbenv global 2.3.1
    ```

1. Install bundler

  ```
  gem install bundler
  rbenv rehash
  ```

1. Install gems

  ```
  bundle install
  ```

1. Set up your local database

  ```
  bundle exec rake db:setup
  ```

1. Run the server

  ```
  bundle exec rails s
  ```

1. Go to localhost:3000

  ```
  http://localhost:3000/
  ```
