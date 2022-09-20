# tailwind-boilerplate
TailwindCSS Boilerplate with additional supporting files.<br>
# Run The Build: <br>
**Step 1**<br>
```bash
  npm i -D tailwindcss
```
**Step 2**<br>
```bash
  npm run build
```
**After that run the live server or open the html page to check if it is working**
<br><br>
# Full Installation Process[From the Scratch]<br>
1. `npm init -y` [Initializing node project.creates package.json file]
2. `npm i -D tailwindcss` [installing tailwindcss as developer dependency.Creates node_modules and package-lock.json file]
3. tailwindcss intellisense vs code plugin installing
4. `npx tailwindcss init --full` [making configuration file for tailwindcss and for its customization. --full gives all default values(use of `--full` is optional)]
5. create src and output folder
6. create a css file in the src folder
7. add tailwind directives to src css file
8. create **.vscode/settings.json** file [to write custom settings of vs code]
9. add
`{
    "css.validate": false,
    "tailwindCSS.emmetCompletions":true
}`
10. update these specific package.json file with -
`"scripts": {
    "build":"tailwindcss -i ./src/input.css -o ./dist/output.css -w"
 },`
11. link html with output css file-
`<link rel="stylesheet" href="../dist/output.css">`
12. update the content line of tailwind.config.js file with this -
`content: ["./src/**/*.{html,js}"],`
13. `npm run build` [this will compile the input file to generate the output file and will keep watching for changes]

# Version
- [TailwindCSS v3.1.8](https://tailwindcss.com/docs/installation)
