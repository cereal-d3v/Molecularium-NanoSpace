## Run in the attractions directory
`cd NanoSpace/server/public/attractions`
## First run this command to preview changes 
`find . -name "index.html" -exec grep -H "back_to_nav" {} \;`

## Then run command to change nanospace button reference to back button

`find . -name "index.html" -exec sed -i '' 's|href="../../#arcade"|href="javascript:history.back();"|g' {} \;`