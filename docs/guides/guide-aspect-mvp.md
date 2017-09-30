# `Aspect like MVP`

Here it is all on one place.
Wicht this approach you have everything of this "aspect"
at one place in the project to work with.

- Aspect "User Configuration"
    - View (Link to View in ViewLayer)
    - ViewModel (Link to ViewModel in ViewLayer)
    - Presenter (Link to Presenter in ViewLayer)
    - Model (Link to Model in Businesslayer)
    - ModelStorage (Link to ModelStorage in DataLayer)

Here it is in each layer (project, Dll)

- ViewLayer (.proj, DLL, Lib)
    - View
        - UserConfigurationView
    - ViewModel
        - UserConfigurationViewModel
    - Presenter
        - UserConfigurationPresenter
- BusinessLayer (.proj, DLL, Lib)
    - Commands
        - AddUserCmd
        - DeleteUserCmd
        - ChangeUserCmd
    - Model
        - User
- DataLayer (.proj, DLL, Lib)
    - ModelStorage(DB, File, WebService, WebApi, ...)
        - UserDbStorage
        - UserFileStorage
        - UserWcfStorage
        - UserWebApiStorage


## Introduction

Lorem markdownum utroque inmittitur fregit omnis ritus **iniquae umero edere**
hamos, confugisse sit venae quis herbas. Vir arbore cetera auctor, sed de hos.
Titulus solvere **dolet** pater visa fetum fata fecit sorbentur inane

## Solution

Lorem markdownum utroque inmittitur fregit omnis ritus **iniquae umero edere**
hamos, confugisse sit venae quis herbas. Vir arbore cetera auctor, sed de hos.
Titulus solvere **dolet** pater visa fetum fata fecit sorbentur inane

## Problem

Lorem markdownum utroque inmittitur fregit omnis ritus **iniquae umero edere**
hamos, confugisse sit venae quis herbas. Vir arbore cetera auctor, sed de hos.
Titulus solvere **dolet** pater visa fetum fata fecit sorbentur inane