#IP-change

Python script to detect if external IP address has changed.

## How to use

You can directly run this script to check if your external IP address has changed.

Everytime the script runs,
it gets the external IP address for any of the available services in the script.
If the IP is different from the one stored in the temporary file `/tmp/ip.log` 
the script will return an error output (exit 1). 
If it is still the same it will return a normal error (exit 0)

## Integration in Jenkins

You can run the script in Jenkins fetching it from the repository, 
or just copying the script to your Jenkins server.

Then you can enable the email notification on failures to get an email everytime the IP changes.

More details in the [coconauts blog](TODO)