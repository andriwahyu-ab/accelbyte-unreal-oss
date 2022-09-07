# Changelog

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

### [0.5.4](https://bitbucket.org/andriwahyu/justice-ue4-oss/branches/compare/0.5.4%0D0.5.3) (2022-09-07)


### Features

* add feature ([9827d3e](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/9827d3e22c00403fc36f2fa73a4f458ac855e27c))
* add new feature ([98d4c7e](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/98d4c7ed571b759a8da4d440547aa3b4217c75c4))

### [0.5.3](https://bitbucket.org/andriwahyu/justice-ue4-oss/branches/compare/0.5.3%0D0.5.2) (2022-09-05)


### Features

* hotfix ([a17a6a1](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/a17a6a185eb7b201cce6d5ea96b1c23ee4040c96))

### [0.5.2](https://bitbucket.org/andriwahyu/justice-ue4-oss/branches/compare/0.5.2%0D0.5.1) (2022-09-05)


### Features

* hotfix ([5b0a1ac](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/5b0a1ac084f47a0a0a177948ba2ee8dff7ee7dc2))

### [0.5.1](https://bitbucket.org/andriwahyu/justice-ue4-oss/branches/compare/0.5.1%0D0.5.0) (2022-09-04)


### Features

* **commerce:** Entitlement, Purchase, Store Interfaces ([572868d](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/572868dc20d7b9ea5d0f7aec8e51021deeb36366))
* **entitlement:** add platform iap sync ([1198e67](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/1198e67a1c8b9971640f15e8ee88df638559855d))
* **entitlement:** add sync dlc ([bad1bde](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/bad1bde1b8a35e131906b282a26cb526d4bf2a86))
* **purchase:** add redeem code ([a2d9f64](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/a2d9f64573ff5c882280f403bfb69a6ebcd65f30))
* **purchase:** add some adjustment on checkout ([027db5d](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/027db5d432b09c2f59c96f945e02fcdf7bdeba4e))
* **store:** add query offer by offer id ([1414141](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/141414114685de9fb5278d8766a5ad2f2fa09c90))
* **Subsystem:** move Get language from store interface to subsystem ([50b6af1](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/50b6af1e476e54918577c18d469a9d094e724dc7))
* update submodule ([18f3bd8](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/18f3bd81ff0c54907a89201e1eaaf0b8efef9562))
* update tag ([37d8bc1](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/37d8bc11a83c71c9e6bbccd20bbd3e5dd5322c0d))


### Bug Fixes

* change SetPartyLeaveNotifDelegate to SetPartyMemberLeaveNotifDelegate due to deprecation of PartyLeaveNotif delegate ([ee120de](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/ee120deef68862472520861283b2c548516d538c))
* **core:** fix some typo that detected on linux build ([cf67aa6](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/cf67aa65e17cf1a2b942a6fe5e84f9dce5b99991))
* gitmodules to pointing andriwahyu repos ([db8fe80](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/db8fe803122e4a5d79bc22536d46a310ef384299))
* **purchase:** change error message to reflect BE error ([c6fb5ea](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/c6fb5ea0fc0c16d8110e9b9bb23fe44ffe7afda2))
* **store:** some adjustment on query categories ([e88dce1](https://bitbucket.org/andriwahyu/justice-ue4-oss/commits/e88dce13baedfa75ad128ed82010fbedd9015346))

## 0.5.0 (2022-08-22)

### Bug fixes

* **session:** joinable session not working due to enqueue session is not implemented
* **identity:** lobby websocket not disconnected during logout

## 0.4.1 (2022-08-05)

### Bug fixes

* **oss:** fix racing condition when the same user is logging in and out consecutively in short period of time

## 0.4.0 (2022-08-02)

### ⚠ BREAKING CHANGES

* **oss:** remove singleton instance for several Online Interfaces to run in PIE mode
* **oss:** move SetLocalUserNumCached, GetLocalUserNumCached and GetApiClient from Online Identity interface to the Subsystem class 

### Features

* **identity:** add new config bMultipleLocalUsersEnabled to enable or disable multiple local users support

## 0.3.1 (2022-07-21)

### Bug fixes

* **identity:** fix login with refresh token type

## 0.3.0 (2022-07-18)

### Features

* **wallet:** implement Online Wallet Interfaces which handle AccelByte Wallet services
* **oss:** now supports UE5
* **session:** trigger delegates on failed matchmaking

### Bug fixes

* **session:** fix End Session to support matchmaking and p2p game session
* **session:** fix Register and Unregister player to session
* **session:** fix joinable game session
* **party:** fix Online Party Interfaces implementation

## 0.2.2 (2022-07-12)

### Bug fixes

* **linux build:** fix linux build, move static struct outside the online agreement class

## 0.2.1 (2022-07-05)

### Bug fixes

* **lobby:** fix trigger on connect lobby always return false

## 0.2.0 (2022-07-04)

### Features

* **agreement:** implement Online Agreement Interfaces which handle AccelByte Agreement services

### Bug fixes

* **presence:** player unable to set presence status

## 0.1.0 (2022-06-06)

### Features

* **identity:** implement Online Identity Interfaces such as login, logout and player profiles
* **party:** implement Online Party Interfaces such as create party, kick member, etc. 
* **friends:** implement Online Friend Interfaces such as add and remove friends
* **presence:** implement Online Presence Interfaces such as set presence status
* **session:** implement Onlinbe Session Interfaces such as start matchmaking, create session, find sessions, join session, etc. 
