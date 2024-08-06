# kodey-vue-jest-test-sample

This repository is an example Kodey.ai Coding Agent Workflow

## Objectives

In this sample, we will explore how Kodey.ai can create jest test cases for vue based applications.

## Project Setup & Steps 

1. Signup for a new Kodey.ai account or login to your existing Kodey.ai environmenty (link-here)
2. Configure your Kodey.ai integrations to the desired issue tracker and cloud git provider.
3. Fork this repository, and clone it to the cloud git provider of your choosing (Github, Azure DevOps, Bitbucket)
4. Make sure you have dev branch. If not create one, kodey will be creating all the new branches against dev.
5. Create the sample issue / work item in your issue tracker. Copy and Paste the issue description from below.
6. Execute the below prompt in the Kodey.ai chat UI
7. Validate the commits and pull requests in your cloud git provider

### SAMPLE PROMPT - Jest Test Cases For Vue Based Applications
```
        platform: github | bitbucket | azure | gitlab (choose one of these)

        project-to-work-on: kodey-vue-jest-test-sample (ONLY IF AZURE)
    
        repository-to-work-on: kodey-vue-jest-test-sample
    
        branch name to create: tests/unit-test-cases-v1
      
        programming language: typescript

        Information to agent: Do as the steps below are defined one by one. You are working in github repo so make sure to use tools related to github repo.

        Scenario: You should write the actual implementation of code not just comments. You are working to develop the test cases unit test scripts using jest framework for an application based on vue framework. The components and functions code will be provided to you and you have to come up with the test scripts for them.

        Steps:

        step 1: Create a new branch with name <branch name to create> and then do the steps below.

        step 2: Get the content of the file src/views/Tab2Page.vue, and understand what this file is responsible for and what are the functions and components being used.

        step 3: Get the content of the file src/composables/usePhotoGallery.ts, this file contains all the functions and logic that are being applied to our above vue components. Understand what each function is doing and how they are implemented also understand how to import the functions and components from it to be used later when creating test scripts. You should understand what are the functions and constants.

        step 4: Now create a new file in tests/unit/ which will have the test cases logic in it for testing the functions used in step 3. NOTE: Make sure to import the components and functions in a syntactically correct way. Please use mount instead of shallowMount when creating wrapper for the component. provide full code with testing logics not just comments.

        step 5: Create a new Pull Request from the above created branch with title "Test Cases Developed v1" and body "Test cases developed with kodey v1".

        step 6: Update this issue status to closed.
```

## Once you have set the description of the issue in your relavant system. You need to use kodey UI Chat and execute below statement to get the work done. 

### Github Issue and Github Repo
```
   Get the issue with id <issue_id> from github repo and do as the description of the issue says step by step.
```

### Azure Repo Issue and Azure Repo
```
   Get the issue with id <issue_id> from azure repo and do as the description of the issue says step by step.
```

### Jira Issue and Bitbucket Repo
```
   Get the issue with id <issue_id> from jira and do as the description of the issue says step by step.
```

## Confirming Successful Sample Outputs

1. Confirm that the branch was created on the issue / work item
2. Confirm that the code created in the associated pull request contains the following
3. Confirm that the work item/issue/ticket in your relevant issue tracking platform is updated.