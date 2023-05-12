# defaul-ssl-profile-script
SSL default profiles
Net Scaler appliances come with two in-built default profiles –

ns_default_ssl_profile_frontend – default front-end profile for all SSL type virtual servers and Internal services.

ns_default_ssl_profile_backend – default back-end profile for SSL type services, service groups, and secure monitors.

Any new endpoint created gets corresponding default SSL profile bound.

It is possible to change the SSL parameters and ciphers of default SSL profiles. This ensures that customers can change the settings and bindings at one point which gets referenced by corresponding endpoints.

This repository contains a python script that will export a list of the SSL vServers on a NetScaler appliance, and will assist witht he creation of a script that will assign a default SSL profile to this list of vServers.
