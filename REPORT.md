## The two microservices are running and registered (two terminals, logs screenshots).

Accounts service running on port 2222

![Accounts log](screenshots/accounts_service_2222.png)

Web service running on port 3333

![Web log](screenshots/web_service_3333.png)

## The service registration service has the two microservices registered (a third terminal, dashboard screenshots)

Registration server running on port 1111

![Registration log](screenshots/registration_service_1111.png)

Eureka dashboard on http://localhost:1111

![Registration dashboard](screenshots/eureka_dashboard.png)

## A second account microservice is running in the port 4444 and it is registered (a fourth terminal, log screenshots).

Accounts service running on port 2222

![Accounts log](screenshots/acounts_service_4444.png)

Eureka dashboard on http://localhost:1111

![Registration dashboard](screenshots/eureka_dashboard_2.png)

## A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?

We will kill the microservice account 2222, and we will get an error if we try to access this service via web.

![Accounts error](screenshots/Accounts_2222_killed.png)

If we wait, the changes will spread and Eureka will recover the account in the port 4444 and it will continue to work

![Recovered accounts](screenshots/recovered_accounts.png)