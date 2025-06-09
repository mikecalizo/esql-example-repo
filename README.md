# esql-example-repo
These ar collection of demo artifacts for ES|QL

Use-cases:

- Monitoring Staff accessing DGA domains over several hours. As SOC team, they see DGA domains frequently and some of it is just ad-tracking. With them using ES|QL they can spot machines that are accessing DGA domains over multiple hours which may indicate malware on their device. - This is what we troubleshoot yesterday.
- Similarly the firewalls do classify some domains as cryptomining that a user may just stumble across. They use ES|QL to keep an eye on the devices that are consistently accessing cyrptomining domains and therefore may have cyrptomining software or malware installed.
- At risk users. They have methods to calculate a logarithmically weighted metric that reflects the number of "newly observed" domains a user accesses vs the amount of unique hours they access them across. This used to be a dashboard they checked daily, but now they can do this with an alerting rule as ES|QL allows us to set much more complex thresholds rather than just document count > X.
