JupyterHub

YouTube https://youtu.be/LkgSCjyv75s

0:00 Welcome and Intro

0:01:00 GitHub repo that accompanies the talk

0:01:44 What is the Notebook?

0:03:00 What is a Notebook Server?

0:04:17 JupyterHub

0:05:41 Login

0:05:55 Spawner

0:06:27 Proxy

0:07:11 Redirect user

0:07:17 Browser to ask hub for auth

0:07:56 Installation (as admin)

0:10:44 Installation (this repo)

0:11:18 Installation: Caveats

0:12:18 conda-forge - community maintained conda packages
   Add conda-forge to default conda sources

0:13:38 Installation docker (later on)

0:14:18 JupyterHub Defaults
    Default behavior
    Auth: PAM
    Spawning: Local users
    Hub run as root (alternative: sudospawner is fraught with peril)

0:15:12 Type jupyterhub in terminal
    jupyterhub SSL

    If you want to run without SSL.

0:16:26 SSL
    self signed cert

    Let's Encrypt 17:30

0:18:12 Configure jupyterhub
    create file
    edit file 19:12

0:20:33 Connect to hub publicly
    login, spawn server, redirect
    control panel 21:20 elaborate!

21:52 Installing kernels for all users

24:15 Using GitHub OAuth
    We have simple PAM; tell server to use GitHub OAuth
    Authorization callback URL
    Client ID
    Client Secret

    ./env -> export the variables

30:44 Tell Jupyter to use oauthenticator

32:48 Sign in with GitHub

34:20 Specifying users
    PAM ok
    GitHub probably not ok
    user whitelist - python set
    admin users - python set

36:26 Jupyterhub Custom Authenticators
    PAM - form based fairly simple
    Secure Authenticator
    jupyterhub hashing salted functions

42:14 Using DockerSpawner
    netifaces convenience thing
    local GH to general GH users
    GH - DockerSpawner
    and whitelist

44:00 Initially missing piece Hub API if cookie is valid
    docker0 ip address netifaces

48:00 Lots you can do with DockerSpawner

51:19 Customizing JupyterHub Spawners
   Start my server goes to a form

1:07 JupyterHub with supervisor

1:09 Reference deployments

1:11:00 Q & A

1:13:00 Simula deployment with persistence in Hub

