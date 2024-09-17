CLI tips

the following command would bind the message parameter to "goodbye world" instead of the default "hello world" in parameters.yml

argo submit arguments-parameters.yaml -p message="goodbye world"

In case of multiple parameters that can be overridden, the argo CLI provides a command to load parameters files in YAML or JSON format. Here is an example of that kind of parameter file:

message: goodbye world
To run use following command:

argo submit arguments-parameters.yaml --parameter-file params.yaml

specify an entrey point like this:
argo submit arguments-parameters.yaml --entrypoint whalesay-caps

