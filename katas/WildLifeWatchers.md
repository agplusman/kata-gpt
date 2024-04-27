(O'Reilly Autumn/Fall 2023)
# Requirements Overview
Wildlife AI is a charitable trust using AI for wildlife conservation. Wildlife.ai work with grassroots wildlife conservation projects and develop open-source solutions using machine learning. They also organise community events, seminars and educational activities to build and maintain machine learning solutions to reduce the current rate of species extinction.

## Assumptions
We assume that a thorough vetting process is applied for accepting users onto the platform to ensure, as much as possible, that information regarding animals location and numbers are not made available to animal poachers and other such criminal organisations. We expect this facility to be in place as it will be very difficult for the application to ensure the user's genuine reasons for requesting such information.
Start with a mobile client and a web application. Same responsive and adaptive application (BFFs might be used in the future)
Observability using Cloud native solutions at the beginning. No particular reporting needs but the solution should accommodate such requirements in the future.
Wildlife.ai users are allowed to buy a camera and install it wherever they consider appropriate, to spot specific wildlife
## Considerations
Cameras will have to have the ability of connecting to a message broker using IoT protocols MQTT would be preferable.
Cameras will be programmed to send a heartbeat message at regular intervals for as long as they are live.
Cameras are pre-configured and ready to connect to the platform. The only requirement for the user installing the camera is to purchase a mobile data SIM card and plug it into the camera before turning it on.
## Use Cases
Identify wildlife in an image and retain necessary information for future research.
* View device(camera) information
* Device self-registration
* Device-User association. If I buy a camera I want to be the one allowed to manage it, along-side the Wildelife.ai administrators
* Analyse Images
* Analyse video
* Observability - Monitoring and alerting for device status as well as whole system availability
## Risks
Animal poachers or such criminals can take advantage of the information made available through this solution
Cameras may not have the necessary hardware capabilities to connect to the message broker for heartbeat and updates so more manual interventions required
