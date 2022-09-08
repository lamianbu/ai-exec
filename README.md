# ai-exec
A global command for Node.js to execute Javascript code string, like eval().
# example1
copyFile in command line.
```cmd
npx ai-exec "require('fs').copyFileSync('./src.txt', './dest.txt');"
```
# example2
exec 'npm i' if not exists 'node_modules'.
```cmd
npx ai-exec "if(require('fs').existsSync('node_modules')){}else{require('child_process').execSync('npm i', { stdio: 'inherit' });}"
```

