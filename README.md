# GA_NodeREDTrigger

See the provided flow to check for new alarms.

## Workflow
Click on Start to activate the 10s poll intervall. Click on Stop to halt it again.

It always retrieves the full list of alarms. It seems like ```alarms[0]``` is always the must recent one, so it just parses the date of this one. Should it match the time in the intervall 0-30s difference, then the alarm trigger sends ```true``` to the output where you may attach your application.

## Things you must change for your setup
You must provde your personal access token for the API generated in your account. Replace the ```myAccessToken``` in the RequestGenerator with your Token.
