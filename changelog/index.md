# change log

## 1.14.0

*2023-05-25*
### New features
- Horizontal sidebar
- [Support monitor execute script #51](https://github.com/zhenorzz/goploy/pull/51)
- [Support project tag #51](https://github.com/zhenorzz/goploy/pull/51)
- [Add nginx manage #52](https://github.com/zhenorzz/goploy/pull/52)
- Support sftp copy rename edit file

### Optimization
- Add app version in login page
- Optimize code

### Bug fixed
- [Jump server #54](https://github.com/zhenorzz/goploy/pull/54)
- Ping db after open connection
- Fix page css

## 1.13.1

*2023-04-29*
### Bug fixed
- Fix windows mkdir
- Refresh file sync project list 
- [Fix check monitor config](https://github.com/zhenorzz/goploy/commit/dae371d96cbf241c4dbf9776c48dc1611e4dcff1)
- [Support sftp --delete option](https://github.com/zhenorzz/goploy/commit/5a0092412151212cab4adc8ca3d589eddb279645)
- [Fix monitor can not redo the task](https://github.com/zhenorzz/goploy/commit/4db5bd6f7bcfa4e647d923d10a59504548408e37)

## 1.13.0

*2023-03-03*
### New features
- Batch execute script

### Optimization
- Show server name in monitor table

### Bug fixed
- Navbar dark mode
- Windows ssh connect

## 1.12.3

*2023-02-03*
### Optimization
- Adjust commit list table column
- Refactor code
- Update Server process list UI

### Bug fixed
- Server process output newline

## 1.12.2

*2022-11-02*
### Optimization
- Support delete file via sftp

### Bug fixed
- Key column 'server_id' doesn't exist in table


## 1.12.1

*2022-10-22*
### Optimization
- Support double click for sftp directory
- Update package.json

### Bug fixed
- Translation
- Dark mode
## 1.12.0

*2022-10-11*
### New features
- Third login
- Transfer file across server

### Optimization
- SFTP support mutiple server
- Server process manage

### Bug fixed
- Xterm disconnect before unmount

## 1.11.0

*2022-09-19*
### New features
- Notify tag after deploy
- Operation log
- serial/parallel publish to server

### Bug fixed
- Fix after deploy script

## 1.10.0

*2022-08-31*
### New features
- Server process manager
- Customize project transfer protocol

### Optimization
- Tag view UI
- Support more predefined vars

## 1.9.1

*2022-08-16*
### Bug fixed
- Fix dockerfile
- Fix bat newline
- Fix sftp dropdown

## 1.9.0

*2022-07-11*
### New features
- Dark mode

### Optimization
- Sidebar 

## 1.8.1

*2022-07-02*
### New features
- Support after deploy script replace commit info

### Bug fixed
- Fix svn commit list

## 1.8.0

*2022-05-17*
### New features
- Support sftp transfer files
- Show deploy detail in realtime

### Bug fixed
- fix deploy list remove item failed
- fix ftp login anonymous

## 1.7.1

*2022-05-09*
### Optimization
- show server on edit monitor item

### Bug fixed
- fix ace editor not found
- fix monitor nil pointer


## 1.7.0

*2022-04-29*
### New features
- Monitor

## 1.6.1

*2022-04-20*
### New features
- Support password login ssh (only work in linux)

### Bug fixed
- fix web script editor

## 1.6.0

*2022-04-11*
### New features
- RBAC

## 1.5.0

*2022-03-24*
### New features
- detect project name is link
- import csv in server page
- install agent in server page

### Optimization
- update element-plus to 2.0
- goploy-agent check sign
- project dialog modify server and user
- file sync move to deploy page

### Bug fixed
- fix vue3 SFCs ref undefined
- fix cron task date popover
- fix publish detail filter popover
- fix namespace add user

## 1.4.7

*2022-03-14*
### New features
- support deploy ftp & sftp

### Optimization
- script setup SFCs
- migrate docs to goploy-devops/goploy-doc

### Bug fixed
- sftp file upload

## 1.4.6

*2022-02-24*
### New features
- web log
- sftp file preview

### Bug fixed
- web cookies undefined 

## 1.4.5

*2022-01-26*

### New features
- new web shell
- new sftp
- support copy server config

### Bug fixed
- git current branch

## 1.4.4

*2022-01-17*

### New features
- support jump server
- process manager
- split log

### Optimization
- decode query

## 1.4.3

*2021-12-24*

### Optimization
- code
- select db
### Bug fixes
- fix exit deploy script
- fix tag refresh
- fix deploy filter
- fix file upload

## 1.4.2

*2021-12-15*

### New features
- .env -> goploy.toml
- support ldap

### Bug fixes
- fix 飞书构建通知

## 1.4.1

*2021-12-09*

### New features
- file compare

## 1.4.0

*2021-12-04*

### New features
- second's cron 
- support svn hook

### Optimization
- route

### Bug fixes
- svn commit id length

## 1.3.8

*2021-11-20*

### New features
- server notify
- send command to all xterm

### Optimization
- ts type

### Bug fixes
- fix web re-login

## 1.3.7

*2021-11-09*

### New features
- monitor server performance  

### Bug fixes
- fix web redirect
- fix web date select i18n

## 1.3.6

*2021-10-15*

### New features
- monitor support http

### Optimization
- delete cache

### Bug fixes
- fix task block
- fix symlink rollback

## 1.3.5

*2021-09-18*

### New features
- allow sort server ip
- add server configuration
- support multiple browser tabs

### Optimization
- fix vite hot reload

## 1.3.4

*2021-08-20*

### New features
- support update app version
- support svn
- customize symlink backup number
- add cmd mode in pull script 

### Optimization
- repository factory (for support other protocol in the future)

## 1.3.3

*2021-07-16*

### New features
- web sftp
- support deploy table sorting

## 1.3.2

*2021-06-25*

### Optimization
- web ssh

### Bug fixes
- fix illegal namespace
- fix web keep alive
- fix copy public key

## 1.3.1

*2021-05-30*

### Optimization
- vite + vue3 + ts
- mobile compatible

### Bug fixes
- symlink in docker
- placeholder

## 1.2.2

*2021-03-26*

### Optimization
- go embed static file
- more notify content

### Bug fixes
- fix symlink rollback

## 1.2.1

*2021-03-03*

### New features
- server terminal
- server can stay in any namespace 

### Optimization
- http.put for edit

### Bug fixes
- fix wss protocol
- delete trim rsync option

## 1.1.6

*2021-02-12*

### New features
- add ssh key path
- server host supports domain
- support graceful stop
- support symlink rebuild

### Optimization
- add git url tips
- delete server install module

## 1.1.5

*2021-01-20*

### Optimization
- deploy detail filters

### Bug fixes
- fix detail loading
- fix missing sql

## 1.1.4

*2021-01-07*

### New features
- add flag --asset-dir=

### Optimization
- delete rsync option --delete-after
- unique project file

### Bug fixes
- fix copy project
- fix refresh tag view
- fix ssh fingerprint

## 1.1.3

*2021-01-06*

### New features
- upload project file

## 1.1.2

*2020-12-26*

### New features
- tags view

### Bug fixes
- fix get detail timeout

## 1.1.1

*2020-12-03*

### New features
- branch deploy

## 1.0.7

*2020-11-27*

### New features
- reset deploy state

## 1.0.6

*2020-11-07*

### New features
- grey publish

## 1.0.5

*2020-11-06*

### New features
- deploy tag list
- predefined vars 

## 1.0.4

*2020-10-25*

### New features
- Project review

### Bug fixes
- Fix monitor bug

## 1.0.3

*2020-10-11*

### New features
- Monitor
  - notify times
  - error content

### Bug fixes
- Fix monitor bug

### Optimization
- table loading

## 1.0.2

*2020-09-04*

### New features
- I18n

### Bug fixes
- Fix SQL error

### Optimization
- project path 
  - change project_name to project_id

## 1.0.1

*2020-08-21*

### New features
- namespace

### Optimization
- Auto deploy
  - change project_name to project_id
