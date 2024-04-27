(O'Reilly Autumn/Fall 2023)
# Requirements Overview

Wildlife AI is a charitable trust using AI for wildlife conservation. Wildlife.ai work with grassroots wildlife conservation projects and develop open-source solutions using machine learning. They also 
organise community events, seminars and educational activities to build and maintain machine learning solutions to reduce the current rate of species extinction.

# Assumptions

* We assume that a thorough vetting process is applied for accepting users onto the platform to ensure, as much as possible, that information regarding animals location and numbers are not made available to animal poachers and other such criminal organisations. We expect this facility to be in place as it will be very difficult for the application to ensure the user's genuine reasons for requesting such information.
* Start with a mobile client and a web application. Same responsive and adaptive application (BFFs might be used in the future)
* Observability using Cloud native solutions at the beginning. No particular reporting needs but the solution should accommodate such requirements in the future.
* Wildlife.ai users are allowed to buy a camera and install it wherever they consider appropriate, to spot specific wildlife

# Considerations

* Cameras will have to have the ability of connecting to a message broker using IoT protocols MQTT would be preferable. 
* Cameras will be programmed to send a heartbeat message at regular intervals for as long as they are live.
* Cameras are pre-configured and ready to connect to the platform. The only requirement for the user installing the camera is to purchase a mobile data SIM card and plug it into the camera before turning it on.

# Use Cases

* Identify wildlife in an image and retain necessary information for future research.
* View device(camera) information
* Device self-registration
* Device-User association. If I buy a camera I want to be the one allowed to manage it, along-side the Wildelife.ai administrators
* Analyse Images
* Analyse video
* Observability - Monitoring and alerting for device status as well as whole system availability

# Risks

* Animal poachers or such criminals can take advantage of the information made available through this solution
* Cameras may not have the necessary hardware capabilities to connect to the message broker for heartbeat and updates so more manual interventions required

# Prioritised Architecture Characteristics ("illities")

## Extensibility
Wildlife.AI will encourage its community of users to purchase and install cameras in the wild, especially in places and regions where there might be endangered species or other rare wildlife. Therefore, Wildlife.AI could potentially deploy a large number of these cameras in the wild and, in the future, may allow other devices to be registered as long as they can provide the necessary information via the connectivity channels available. 

## Total Cost
Wildlife.ai are a non-profit organisation and thus any solution proposed must be cost-effective and not incur unnecessary expenses such as third party licenses or "idle" runtime costs. The proposed solution must allow for the use of Elastic cloud technologies. The implementation of this architecture must follow the cloud-native patterns.

## Scalability
The architecture must ensure that the system can accommodate an increasing number of cameras. People can buy and install cameras at their own expense, so the solution must be able to accommodate these cameras when they come online.
The application must also allow for a growing number of users, both regular users and camera administrators, to subscribe and operate on the platform.

## Security & Privacy
Access to the data captures regarding animals locations and other such details represent important pieces of information for the future of animals concerned. Therefore, a thorough vetting process must be applied for accepting users onto the platform. The user registration process must have 3 stages: 
1. Registration - users register and submit the required documentation
2. Vetting - Wildlife.ai ensures that the person wanting to use the platform has been properly verified.
3. Activation - After the user has been vetted and allowed onto the platform an activation email and unique URL are being generated so that the user can finalise the activation process.
The system must be secure so that the information regarding camera locations as well as Observations should only be accessible to screened users.
All data navigating through our solution is backed by latest TLS version and we recommend employing data repositories that can encrypt data at rest.
