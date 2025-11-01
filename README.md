# ap_webflow_videos

readme change


I'm getting this message in vs code:
This action will pull and push commits from and to "origin/main".

Then this
Git: RPC failed; HTTP 400 curl 56 The requested URL returned error: 400

I think it's cuz movie is big. large file size.

Solved by this
https://stackoverflow.com/questions/62753648/git-push-failure-while-pushing-a-large-respository-of-code

do this:
git config http.postBuffer 524288000
followed by

git pull && git push

—

Use this and then video name
ap-webflow-videos.netlify.app


so it should look like this:ap-webflow-videos.netlify.app/Design_token_cs.mp4

Then make html embed:
<video id="video" playsinline loop muted style="width: 100%;">
	<source src="https://ap-webflow-videos.netlify.app/websiteBuilder_cs_homepage.mp4" type="video/mp4">
</video>