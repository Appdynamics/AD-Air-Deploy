# AD-Air-Deploy

If deployed to AWS, use something like a t3.large or t3.xlarge linux instance.

Dependencies:
docker
docker-compose
git

Update controller.env:

APPDYNAMICS_AGENT_ACCOUNT_ACCESS_KEY= # Access Key from controller
APPDYNAMICS_AGENT_ACCOUNT_NAME=customer1
APPDYNAMICS_AGENT_APPLICATION_NAME=AD-Air
APPDYNAMICS_CONTROLLER_HOST_NAME= # controller host IP or DNS. Do NOT add http:// to beginning or port at the end
APPDYNAMICS_CONTROLLER_PORT=8090
APPDYNAMICS_CONTROLLER_SSL_ENABLED=false
EVENT_ENDPOINT= # Optional, but required for Analytics: IP or DNS of Event Service. Do NOT add http:// to beginning, but make sure to include port at the end
FULL_ACCOUNT_NAME=  # Optional, but required for Analytics. Global Account Name	from controller
EUM_HOST= # Optional: IP or DNS of EUM Server. Do NOT add http:// to beginning, but make sure to include port at the end
EUM_KEY= # Optional

# run start.sh

./start.sh
