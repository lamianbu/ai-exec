# ai-exec
A global command for Node.js to exec Javascript code string, like eval().
# example1
'npm i' if not exists 'node_modules'.
```cmd
npx ai-exec "if(require('fs').existsSync('node_modules')){}else{require('child_process').execSync('npm i', { stdio: 'inherit' });}"
```
# example2
'npx shx mkdir dist' if not exists 'dist'.
```cmd
npx ai-exec "if(require('fs').existsSync('dist')){}else{require('child_process').execSync('npx shx mkdir dist', { stdio: 'inherit' });}"
```
