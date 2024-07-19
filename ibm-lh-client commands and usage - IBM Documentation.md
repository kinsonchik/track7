The `ibm-lh-client` package includes utilities for SSL certificate management and engine management.

**watsonx.data Developer edition**

**watsonx.data on Red Hat® OpenShift®**

**watsonx.data SaaS on AWS**

To use the utilities, the `ibm-lh-client` package is to be installed on your system. For more information, see [Installing `ibm-lh-client` package](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd-client/topics/install-lh-client.html)

The `ibm-lh-client` supports the following utilities:

-   [`cert-mgmt`](https://www.ibm.com/docs/en/watsonx/watsonxdata/2.0.x?topic=utilities-lh-client-commands-usage#lh_client_utilities__certificate)
-   [`presto-cli`](https://www.ibm.com/docs/en/watsonx/watsonxdata/2.0.x?topic=utilities-lh-client-commands-usage#lh_client_utilities__presto-cli)
-   [`presto-run`](https://www.ibm.com/docs/en/watsonx/watsonxdata/2.0.x?topic=utilities-lh-client-commands-usage#lh_client_utilities__presto-run)
-   [`python-run`](https://www.ibm.com/docs/en/watsonx/watsonxdata/2.0.x?topic=utilities-lh-client-commands-usage#lh_client_utilities__python-run)
-   [`dev-sandbox`](https://www.ibm.com/docs/en/watsonx/watsonxdata/2.0.x?topic=utilities-lh-client-commands-usage#lh_client_utilities__dev-sandbox)
-   [`ibm-lh`](https://www.ibm.com/docs/en/watsonx/watsonxdata/2.0.x?topic=utilities-lh-client-commands-usage#lh_client_utilities__ibm-lh)
-   [`connect-lh`](https://www.ibm.com/docs/en/watsonx/watsonxdata/2.0.x?topic=utilities-lh-client-commands-usage#lh_client_utilities__engines)

## `cert-mgmt`

Add or remove Presto (Java) engine connection certificates to `ibm-lh-client` truststore.

**Syntax**

Add a Presto (Java) engine connection certificate:

```plaintext
./cert-mgmt --op=add --host=<host> --port=<port>
```

Remove a Presto (Java) engine connection certificate:

```plaintext
./cert-mgmt --op=remove --host=<host> --port=<port>
```

For more information on how to use `cert-mgmt`, refer [Setting up the ibm-lh command-line utility](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd-client/topics/work-ibm-lh.html "The ibm-lh command-line utility provides a terminal interface for issuing the IBM watsonx.data component management and ingestion commands from a client system upon which the CLI utility is installed.")

## `presto-cli`

Start an interactive session.

**Syntax**

Use the following command to start an interactive session:

```plaintext
bin/presto-cli --engine=<engine name> --catalog=tpch
```

For more information on how to use `presto-cli`, refer [Connecting to a Presto (Java) server](https://www.ibm.com/docs/en/SSDZ38_2.0.x/lh-console/topics/con-presto-serv.html "Presto (Java) CLI provides a terminal-based interactive shell to run queries. You can connect to Presto (Java) server either through Presto (Java) CLI installed as part of the ibm-lh-client package or through Presto (Java) CLI installed separately.")

## `presto-run`

Run SQL in a noninteractive manner.

**Syntax**

Use the bin/presto-run utility to run SQL in a noninteractive manner:

```plaintext
bin/presto-run --engine=<engine-name> --catalog=tpch <<< "select * from tiny.customer limit 10;"
```

Run SQL from a file from your LH\_SANDBOX\_DIR mount.

```plaintext
bin/presto-run --engine=<engine-name> -f <path of sql file directory>
```

For more information on how to use `presto-run`, refer [Connecting to a Presto (Java) server](https://www.ibm.com/docs/en/SSDZ38_2.0.x/lh-console/topics/con-presto-serv.html "Presto (Java) CLI provides a terminal-based interactive shell to run queries. You can connect to Presto (Java) server either through Presto (Java) CLI installed as part of the ibm-lh-client package or through Presto (Java) CLI installed separately.")

## `python-run`

It provides a way to run python scripts.

**Syntax**

Start an interactive python session.

```plaintext
bin/python-run --engine=<engine-name>
```

Note: The engine details are available as environment variables (ENG\_HOST, ENG\_PORT, ENG\_USERNAME, ENG\_PASSWORD). For example,`os.environ['ENG_PASSWORD']` provides the saved password for the selected engine.

Run a python script from your LH\_SANDBOX\_DIR mount.

```plaintext
bin/python-run --engine=<lakehouse-engine-name> <python-script-in-sandbox>
```

For more information on how to use `python-run`, refer [Running Python scripts by using ibm-lh-client](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd-client/topics/run-python-lh-client.html "The ibm-lh-client supports the execution of Python scripts.")

## `dev-sandbox`

Provides a containerized environment with useful utilities and python modules to help explore the lakehouse.

**Syntax**

Set the sandbox that starts an interactive bash shell from which you can run other commands:

```plaintext
bin/dev-sandbox --engine=<engine-name>
```

For more information on how to use `dev-sandbox`, refer [Using the developer sandbox container](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd-client/topics/work-container-lh-client.html "You can use the sandbox container to develop various functions by using python and connecting to a Presto (Java) engine.")

## `ibm-lh`

It is a terminal-based interface that is designed to facilitate interaction with watsonx.data resources. For more information on how to use `ibm-lh`, refer [`ibm-lh commands and usage`](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd-client/topics/ibm_lh_commands.html "The ibm-lh command-line utility is a terminal-based interface that is designed to facilitate interaction with watsonx.data resources.")

## `connect-lh`

Manage the connections for your watsonx.data engine. Use this command to add, remove, list, or show details of a Presto (Java) engine connection.

**Syntax**

Add a Presto (Java) engine connection:

```plaintext
connect-lh --op=add \ --name=<alias> \ --host=<host> \ --port=<port> \ --username=<username> \ --password=<password>
```

Remove a Presto (Java) engine connection:

```plaintext
connect-lh --op=remove --name=<alias>
```

Show the connection details for a specific connection:

```plaintext
connect-lh --op=details --name=<alias>
```

List all configured engine connections:

For more information on how to use `connect-lh` refer [Setting up the ibm-lh command-line utility](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd-client/topics/work-ibm-lh.html "The ibm-lh command-line utility provides a terminal interface for issuing the IBM watsonx.data component management and ingestion commands from a client system upon which the CLI utility is installed.")

where:

name

The given name or alias to identify the connection.

For connecting `presto-cli`:

host

IBM watsonx.data developer edition The hostname of the Presto (Java) server.

IBM watsonx.data stand-alone The exposed secure route for Presto (Java) server. For more information, see [Exposing secure route to Presto (Java) server](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd/admin/expose_secure_route.html).

IBM watsonx.data on IBM Cloud Pak for Data The exposed secure route for Presto (Java) server. For more information, see [Exposing secure route to Presto (Java) server](https://www.ibm.com/docs/en/SSDZ38_2.0.x/wxd/admin/expose_secure_route.html).

IBM watsonx.data on IBM Cloud To get the hostname of the Presto (Java) server from the web console, go to Infrastructure Manager, select the engine you want to connect to and copy the host. The copied host contains both the host and port details. Use the host details as the host name of the Presto (Java) server.

For connecting `ibm-lh`:

host

IBM watsonx.data developer edition The hostname of the Presto (Java) server.

IBM watsonx.data stand-alone The hostname of the Presto (Java) server. (You do not need exposed route).

IBM watsonx.data on IBM Cloud Pak for Data The hostname of the Presto (Java) server. (You do not need an exposed route).

IBM watsonx.data on IBM Cloud The hostname of the Cloud server. (For example : us-south.lakehouse.dev.cloud.ibm.com).

For connecting `presto-cli`:

port

The port number of the Presto (Java) server.

IBM watsonx.data developer edition The default port is `9443`.

IBM watsonx.data stand-alone The default port is `443`.

IBM watsonx.data on Cloud Pak for Data The default port is `443`.

IBM watsonx.data on IBM Cloud To get the port number of the Presto (Java) server from the web console, go to Infrastructure Manager, select the engine you want to connect to and copy the host. The copied host contains both the host and port details. Use the port details as the port number of the Presto (Java) server.

For connecting `ibm-lh`:

port

The port number of the Presto (Java) server.

IBM watsonx.data developer edition The default port is `9443`.

IBM watsonx.data stand-alone The default port is `443`.

IBM watsonx.data on Cloud Pak for Data The default port is `443`.

IBM watsonx.data on IBM Cloud The default port is `443`.

username

The username for authentication.

IBM watsonx.data developer edition The default `username` is `ibmlhadmin`.

IBM watsonx.data stand-alone Username is the user created for stand-alone. The default `username` is `admin`. If IAM is enabled, the default user is `cpadmin`.

IBM watsonx.data on Cloud Pak for Data Username is the user created for Cloud Pak for Data. The default `username` is `admin`. If IAM is enabled, the default user is `cpadmin`.

IBM watsonx.data on IBM Cloud Username can either be `ibmlhapikey` or `ibmlhtoken`. For more information on how to use `ibmlhapikey` or `ibmlhtoken`, see [Connect to Presto (Java) server](https://cloud.ibm.com/docs/watsonxdata?topic=watsonxdata-con-presto-serv#conn-to-prestoeng "(Opens in a new tab or window)").

password

The password for authentication.

IBM watsonx.data developer edition The default `password` is `password`.

IBM watsonx.data stand-alone To get the default password for default `admin` or `cpadmin` user, run the following command:

```plaintext
ibm-lakehouse-manage get-cpd-instance-details
```

IBM watsonx.data on Cloud Pak for Data, To get the default password for default `admin` or `cpadmin` user, run the following command:

```bash
cpd-cli manage get-cpd-instance-details \ --cpd_instance_ns=${PROJECT_CPD_INST_OPERANDS} \ --get_admin_initial_credentials=true
```

Note: If the `--password` option is not specified, password is prompted.

IBM watsonx.data on IBM Cloud Password can either be `apikey` or `apitoken`. For more information see, [Get api key](https://cloud.ibm.com/docs/watsonxdata?topic=watsonxdata-con-presto-serv#get-ibmapi-key "(Opens in a new tab or window)") and [Get api token](https://cloud.ibm.com/docs/watsonxdata?topic=watsonxdata-con-presto-serv#get-ibmiam-token "(Opens in a new tab or window)").
