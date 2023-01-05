This is a wrapper script to keep track of my ffmpeg settings I use to transcode videos to be as small as possible for use with my kid's tablet.

<H1>General Use</H1>
Once added to your PATH, use ffmpeg_squish like:
<pre>
ffmpeg_squish input_filename.avi output_filename.mp4
</pre>
The result output file will be as small reaonsably possible for use with smallish tablets.

Note that the file extensions are interpreted by FFMPEG and used. So in the above example, FFMPEG will automatically transcode the container format from AVI to MP4.

<HR>
<H1>General Setup</H1>
<H2>bash/zsh Users</H2>
To add ffmpeg_squish to your path, edit your ~/.bash_profile to update the PATH to include the path to where your copy of ffmpeg_squish is located, for example:
<pre>
...
PATH="/Library/Frameworks/Python.framework/Versions/3.8/bin:${PATH}:/Users/my_username/opt/ffmpeg_squish/bash"
...
</pre>

zsh users (such a more recent macOS users) can get it in their path by updating their ~/.zshrc file with a line like:
<pre>
export PATH="/opt/homebrew/opt/openjdk/bin:/Users/myusername/git/ffmpeg_squish/bash:$PATH"
</pre>
  
<H1>Slack Notifications Setup</H1>
To use slack with ffmpeg_squish, you must set the "FFMPEG_SQUISH_WEBHOOK" environment variable.

<H2>bash users</H2>
For bash users, update your ~/.bash_profile to define FFMPGE_SQUISH_WEBHOOK like:
<pre>
FFMPEG_SQUISH_WEBHOOK="https://hooks.slack.com/services/........"
export FFMPEG_SQUISH_WEBHOOK
</pre>

