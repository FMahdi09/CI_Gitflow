﻿# CI_Gitflow

## User 1:
- git checkout -b feature1
- echo "feature1 first change" >> .\test.txt
- git add .
- git commit -m "feature1 first change"
- echo "feature1 finished" >> .\test.txt
- git add .
- git commit -m "feature1 finished"

## User 2
- git checkout -b feature 2
- echo "feature2 first change" >> .\test.txt
- git add .
- git commit -m "feature2 first change"
- echo "feature2 finished" >> .\test.txt
- git add .
- git commit -m "feature2 finished"

## User 1

- git checkout dev
- git pull
- git checkout feature1
- git merge dev
- git checkout dev
- git merge feature1
- git push

## User 2

- git checkout dev
- git pull
- git checkout feature2
- git merge dev

Resolve Conflict

- git checkout dev
- git merge feature2
- git push 
