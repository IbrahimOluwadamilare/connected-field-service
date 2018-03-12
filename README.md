
<img src="imgs/md/dyn-logo.png">

# Intro to Dynamics 365 Connected Field Service
---
The goal of this repo is to give you everything you need to set up a Connected Field Service (CFS) Environment. using both the first timer recommended [CFS](https://appsource.microsoft.com/en-us/product/dynamics-365/mscrm.58666c7d-65ee-452d-8708-70b4d471d4c0) and more advanced custom Azure deployment.

# Goals
| <p align="center"><img src="imgs/md/code-file.svg" width="64"></p> [1. Provision Dynamics 365](Assets/HoloToolkit/Input/README.md) | <p align="center"><img src="imgs/md/resources.svg" width="64"></p> [2. Provision Azure Trail](Assets/HoloToolkit/Sharing/README.md) | <p align="center"><img src="imgs/md/generics.svg" width="64"></p> [3. Setup MX Chip](Assets/HoloToolkit/SpatialMapping/README.md) |
| :- | :- | :- |
| `{ blurb here }` | `{ blurb here }` | `{ blurb here }` |
| <p align="center"><img src="imgs/md/generics.svg" width="64"></p> [4. Setup MX Chip](Assets/HoloToolkit/SpatialMapping/README.md) | <p align="center"><img src="imgs/md/linq.svg" width="64"></p> [5. Technical decomposition](Assets/HoloToolkit/SpatialUnderstanding/README.md) | <p align="center"><img src="imgs/md/exception.svg" width="64"></p> [6. Something else](Assets/HoloToolkit/SpatialUnderstanding/README.md) |
| `{ blurb here }` | `{ blurb here }` | `{ blurb here }` |

## Finished Product
`{ .gif goes here }`


## Exercise 1: Provision Dynamics 365

1.	From a Web Browser on your computer, visit the [Dynamics 365 for Field Service home page](https://www.microsoft.com/en-us/dynamics365/field-service) and click the `START FREE >` button.

  <img src="imgs/provision-dynfs-homepage.png">

2. Start your digital transformation!
  - `A` Select the Field Service app if it is not selected already
  - `B` Click `Sign up here`

    <img src="imgs/provision-dynfs-fsapp-form.png">

    > IMPORTANT
    >
    > Do not fill out work email and phone number and Do not click `GET STARTED >`

3. Next you'll be naviagted to provision your new Dynamics Trail. Fill out the general information about yourself and your company then click `Next`.

  <img src="imgs/provision-dynfs-personal-info.png">

4. Enter your user ID information and click `Create my account`.

  <img src="imgs/provision-dynfs-user-id.png">

5. Lastly you'll have to confirm your identity using your phone, enter your phone number and click `Text me ->`.

  <img src="imgs/provision-dynfs-phone.png">

6. After phone authentication is complete, you'll be given some important URLS that you should note down while the signup is finishing. Once the signup is finished click the `Set up` that appears.

  <img src="imgs/provision-dynfs-completed.png">

  > NOTE
  >
  > Keep the "Sign-in page" and "user ID" copied somewhere on your computer like a text file, you will need this information later.

7.	Now you should be on the Dynamics 365 FREE 30 Trial set up page.
  - `A` Field service should already be checked, if not make sure to click the check box.
  - `B` Click `Complete Setup`, A "Setting Up..." alert will appear.
  - `C` After the setup is complete you'll get another alert letting you know your Trial Organization will be ready soon!

    <img src="imgs/dyn-free-trial-intro.png">

    <img src="imgs/provision-dynfs-trail-email-alert.png">

8. Head over the [Outlook mail website](https://outlook.office.com/owa/) and sign in with your business email address from step 3. Find the email from Microsoft Dynamics CRM Online and click the `Get Started` button from that email.

  <img src="imgs/dyn-confirmation-email.png">

9. Welcome to Dynamics 365! No let's make sure your account has the right permissions going forward to complete the rest of the exercises we have in store.

  <img src="imgs/dyn-fs.png">

9.	We're going to do this by navigating through our organization's Site Map.
  - `A` Click the drop down arrow next to `Field service`
  - `B` Then click `Settings` to open our system and application settings
  - `C` Click `Security` under System settings

  <img src="imgs/dyn-sitemap-fs.png">

  <img src="imgs/dyn-sitemap-settings.png">

11.	On the Security Settings page Click Users.

  <img src="imgs/dyn-settings-security.png">

12.	On the Enabled Users page:
  - `A` Click the check box next to your name
  - `B` Click `Promote to Admin` button
  - `C` Then click `OK` in the alert dialog that comes up

  <img src="imgs/dyn-settings-security-users.png">

13.	Now that we've provisioned our own Dynamics 365 Online tenant with Field Service installed, we need to provision an Azure environment to host the IoT services for our solution. Keep all of your tabs open and use the same web browser for the following exercises.

> IMPORTANT
>
> Keep all of your tabs open and use the same web browser for the following exercises


## Exercise 2: Provision Azure Trial


1.	On your PC, browse to the [Azure free trail website](https://azure.microsoft.com/en-us/free/) [https://azure.microsoft.com/en-us/free/](https://azure.microsoft.com/en-us/free/) in the same web browser as you.

2.	Click `Start Free >` and sign In with your Dynamics Tenant Trial user ID created in Exercise 1 Step 4 if prompted to do so.

  <img src="imgs/az-free-trial.png">

  > NOTE
  >
  > it will follow this format `Username@TenantName.Onmicrosoft.com`

3.	Fill out steps 1 through in Full through the free account sign up form  .

  <img src="imgs/az-free-trial-signup-one.png">

  <img src="imgs/az-free-trial-signup-two.png">

  <img src="imgs/az-free-trial-signup-three.png">

  <img src="imgs/az-free-trial-signup-four.png">

6.	After agreeing to the terms and clicking `Sign up`, you'll then be navigated to the Azure welcome page. Close this page and head to the [Azure portal](https://portal.azure.com/) at [https://portal.azure.com/](https://portal.azure.com/).

7. Now we have our Azure environment up and running! With both our Azure environment and Dynamics environment in place, all we need now is an IoT device for these platforms to communicate with.

## Exercise 3: Setup MX Chip

`{ TODO }`

## Exercise 4: Configure Connected Field Service (CFS)

1. On your computer, browse to AppSource here [https://appsource.microsoft.com/en-us/product/dynamics-365/mscrm.58666c7d-65ee-452d-8708-70b4d471d4c0](https://appsource.microsoft.com/en-us/product/dynamics-365/mscrm.58666c7d-65ee-452d-8708-70b4d471d4c0) and to download the ["Connected Field Service Add-On"](https://appsource.microsoft.com/en-us/product/dynamics-365/mscrm.58666c7d-65ee-452d-8708-70b4d471d4c0) by clicking `GET IN NOW`. gregdegury@gregdegruy.onmicrosoft.com and https://gregdegruy.crm.dynamics.com/main.aspx#789609347

  <img src="imgs/appsource-cfs-addon.png">

2. You should now see a prompt notifying you that you are being taken to Dynamics 365 to complete the process.

16.	Select the Dynamics 365 Organization
17.	Click Next

18.	Select Azure Subscription
19.	Type a Resource Group Name
20.	Select East US as your Deployment Region
21.	Check PowerBI
a.	Username: PowerBISQL
b.	Password: zaq1@WSX
22.	Click Deploy


23.	Wait while Connected Field Service Deploys
24.	After All of the Resource Deploy, Click the Authorize Button


29.	Clicking the Authorize Button will bring up the API Connection in the Resource Group within the Azure Portal.
30.	Click This connection is not authenticated

31.	Click the Authorize Button

32.	Enter your CRM Credentials (Username@OrganizationName.onmicrosoft.com)
33.	Click Sign In
34.	Click Save

35.	Click on the IoT Hub Item. It is normally named the same as your Resource Group with a GUID after it.

36.	Click on Share Access Policies

37.	Click + to Add a New Shared Access Policy

38.	Give your policy a name: “particle-iot-hub”
39.	 Give your new policy registry read, registry write, and device connect permissions

40.	Click Create to add the new shared access policy. It will take a few moments for Azure to create your new policy successfully.
41.	Click on the Access Policy Name you just created (particle-iot-hub)

42.	Copy the Primary Key to Notepad (Don’t share the Primary Key as it is like giving somebody the keys to your house. Without you home. And Top Shelf Liquor around.)

43.	Go back to the Resource Group
44.	About ¾ the way down the list of resources, there is a App Service that starts with Simulator + words words words words words words words
45.	Click on that resource
46.	Highlight the Resource Name
47.	In a new browser tab, paste the resource name followed by .azurewebsites.net
Like  Simulator.azurewebsites.net
48.
49.	So mine would become: SimulatorCFSHOLb594d2b5d25b48678337857fbe75a3f3.azurewebsites.net


## Exercise 5: Technical Decomposition
`{ will }`

## My Environment
`{ my dynamics and azure environment details }`

# References
- [Connected Field Service Add-On](https://appsource.microsoft.com/en-us/product/dynamics-365/mscrm.58666c7d-65ee-452d-8708-70b4d471d4c0)
- [Connected Field Service Architecture](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/field-service/developer/connected-field-service-architecture)
- [GitHub icons](https://gist.github.com/rxaviers/7360908)
