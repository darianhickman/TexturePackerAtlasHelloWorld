Issues and Resolutions

Initial could not find urls got solved with a new igeRoot
Inside index.html:
<script type="text/javascript">var igeRoot = '/engine/';</script>
<script type="text/javascript" src="/engine/loader.js"></script>
Can’t get web server to serve js files even with obvious urls. 
cd /Users/darianhickman/bitbucket.org/village-makeover
python -m SimpleHTTPServer 9000
spritesheet-1.json
spritesheet-0.json
Resolved a lot not found issues by killing all Chrome windows and restarting.  
Couldn’t mount IgeBaseScene.
ige.addGraph('IgeBaseScene');  ran fine
oh well it’s still referenced by ige.$(‘baseScene’) .  lame design
Some parameter inside TexturePackerAtlas called textureRoot was breaking urls. 
So I removed the parameter form TexturePackerAtlas.js
