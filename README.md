![Logo](./images/orange-logo-w.svg#gh-dark-mode-only)
![Logo](./images/orange-logo-b.svg#gh-light-mode-only)

## Welcome to project orange🟠

### Getting started
If you've just joined project orange🟠, first of all - welcome! Please familiarise with all the information on this meta repo as well as any specific repos you've been assigned to.
Currently, most repos lack technical documentation due to their infancy - however, we've put together a general set-up guide to get you up and running as quickly as possible, no matter which repo you've been assigned to work on.

#### Dev operating system
Most of the software in the orange🟠 stack is written for Node.Js so you can develop on pretty much any platform that supports Node.Js such as:
- Microsoft Windows
- Most GNU/Linux distributions
- Apple macOS
> Our target operating system is typically Ubuntu Server or any RHEL-based server operating system such as Oracle Linux, CentOS, Fedora, etc running on both `linux/amd64` and `linux/arm64` platforms. But this shouldn't matter in most cases as most of the code is portable.
#### Recommended IDE
You can choose which IDE to use, however we'd recommend using VSCode (or a FOSS alternative such as VSCodium). You will need to sign into the GitHub extension to be able to use the version control features to sync your work with the repository. Instructions on how to setup the GitHub integration can be found [here](https://code.visualstudio.com/docs/sourcecontrol/github).
#### Setting up the project
0. Make sure you have the latest version of [Node.Js](https://nodejs.org/) installed.
1. Open a new VSCode window and select *Clone git repository*.

![image](https://github.com/orangegrp/orange/assets/88835216/29a783c0-0d20-44f6-814d-2fd88632fdca)

2. Select *Clone from GitHub* OR *Git: Clone (Recursive)*

![image](https://github.com/orangegrp/orange/assets/88835216/8ebd6430-2849-4402-afc6-060ce2436a89)

3. Select the intended repository. For our example we'll use `orange-bot`.

![image](https://github.com/orangegrp/orange/assets/88835216/a999975f-21aa-4cd7-ad56-2913a3835233)


4. Once the repo is cloned, and you are prompted to open the folder, click *Open*.
5. If you are prompted with a security message asking to trust the author(s), choose *Trust*.
6. Open the built-in VSCode terminal emulator by choosing *Terminal* and then *New Terminal* (or press `CTRL` + `SHIFT` + `'`).
7. In the terminal window, run the setup script by typing `npm run setup`.
8. You can then run `npm run build` to build all the dependencies (you need to do this at least once).
9. From now on, any time you make a change to the code, use `npm run dev` to build and run the current project. If you make any changes to the dependencies, you must run `npm run build` to recompile them.

#### Best practice
It is highly recommended that when working on a new feature, you create your own branch and make your changes there instead of committing to `main`. You can do this by selecting the `main` branch icon at the bottom of VSCode like so:
![image](https://github.com/orangegrp/orange/assets/88835216/a9f45bd0-a08d-4fbd-bb75-8c2a55d9a6aa)

Then click on *Create new branch* and name it accordingly. 
![image](https://github.com/orangegrp/orange/assets/88835216/a5d03d94-d77c-4de2-a430-ce771935cabb)

When you've completed a feature, simply let us know and we'll merge it into the main branch accordingly. If there's any merge conflicts or problems, we'll let you know.

#### 🚨 IMPORTANT 🚨 
Make sure the commit and sync order is correct to ensure the repo refs do not get corrupted! (I learnt this the hard way, thanks Topias for helping me btw).

![image](https://github.com/orangegrp/orange/assets/88835216/9e9908cf-a046-43b6-b7bb-5803c5c3c918)

**Always COMMIT and SYNC** the **submodules FIRST** and only then commit and sync the main repo. (i.e. commit and sync from the bottom-up).
> :warning: Make sure to select a branch for the modules as well, usually `main` is fine. Make sure you can see main instead of the 5857... and cbc3... hashes otherwise you won't be able to sync to the origin.

#### If in doubt, ask
If you're not sure on something, please ask and we'll help you figure it out. 

### List of repositories
| Repo | Description | Status |
| ---- | ----------- | ------ |
| `leta` | (LEGACY BASE) Leta «Лета», the next-generation bot. | ![](https://github.com/orangegrp/leta/actions/workflows/main.yml/badge.svg) ![Static Badge](https://img.shields.io/badge/Sunsetting_in_2024-navy) |
| `studybot` | (LEGACY BASE) | ![Static Badge](https://img.shields.io/badge/Archived-orange) |
| Good Bot | (LEGACY BASE) | ![Static Badge](https://img.shields.io/badge/Unknown-grey) |
| `orange-bot` | orange🟠 Discord Bot | ![](https://github.com/orangegrp/orange-bot/actions/workflows/main.yaml/badge.svg) ![Static Badge](https://img.shields.io/badge/Active_Development-limegreen) ![Static Badge](https://img.shields.io/badge/Latest-beta_0.0.8-limegreen)  |
| `orange-bot-base` | orange🟠 Discord Bot (Base repository) | ![Static Badge](https://img.shields.io/badge/Active_Development-limegreen) |
| `orange-crs` | orange🟠 Code Runner Server | [![orange-crs CI](https://github.com/orangegrp/orange-crs/actions/workflows/main.yaml/badge.svg)](https://github.com/orangegrp/orange-crs/actions/workflows/main.yaml) ![Static Badge](https://img.shields.io/badge/API_v1-Dev_testing-limegreen) |
| `orange-dash` | orange🟠 Dash | ![Static Badge](https://img.shields.io/badge/Early_Development-yellow)  |
| `orange-common-lib` | orange🟠 Common Library and Functions | ![Static Badge](https://img.shields.io/badge/Beta-limegreen)  |

### Team members
| Team member | Actively working on repo |
| ----------- | ------------------------ |
| Topias | orange🟠 Discord Bot (Base repository), orange🟠 Discord Bot, orange🟠 Common Library and Functions |
| Alex | orange🟠 Discord Bot, orange🟠 Common Library and Functions, orange🟠 Code Runner Server, orange🟠 Dash |
| Alastor | orange🟠 Discord Bot |
