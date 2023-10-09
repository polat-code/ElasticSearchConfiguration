# ElasticSearchConfiguration

## Create Container

First, change **image** parameters in **docker-compose.yml** for both elastichsearch and kibana according to your versions.

Go to **docker-compose.yml** directory and Run the following code to code to create a container

```
docker compose up
```

Go to **localhost:5601** and kibernate wants a **enrollment token** . To get **enrollment token** , Run following command in elastic-search command viewed in docker desktop.

```
bin/elasticsearch-create-enrollment-token --scope kibana
```

And paste it into desired input field in web browser.

## Log In

To log in , default user is

Username : elastic \
password : unknown

To get password , Run the following code in elastic-search command viewed docker-desktop.

```
bin/elasticsearch-reset-password -u elastic
```

## View data

Go to **localhost:9200** to see data
