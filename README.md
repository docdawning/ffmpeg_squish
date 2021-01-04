This is a wrapper script to keep track of my ffmpeg settings I use to transcode videos to be as small as possible for use with my kid's tablet.

<H1>General Setup</H1>
<H2>BaSH Users</H2>
To add ffmpeg_squish to your path, edit your ~/.bash_profile to update the PATH to include the path to where your copy of ffmpeg_squish is located, for example:
<pre>
...
PATH="/Library/Frameworks/Python.framework/Versions/3.8/bin:${PATH}:/Users/my_username/opt/ffmpeg_squish/bash"
...
</pre>

<H1>Slack Notifications Setup</H1>
To use slack with ffmpeg_squish, you must set the "FFMPEG_SQUISH_WEBHOOK" environment variable.

<H2>BaSH users</H2>
For bash users, update your ~/.bash_profile to define FFMPGE_SQUISH_WEBHOOK like:
<pre>
FFMPEG_SQUISH_WEBHOOK="https://hooks.slack.com/services/........"
export FFMPEG_SQUISH_WEBHOOK
</pre>

