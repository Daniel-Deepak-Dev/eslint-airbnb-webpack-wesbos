1.eslint:

    file: .eslintrc
        "rules":{
            no-console: 0
        }
        //here 0 is off; 1 is warn; 2 is error 

        "extends": "eslint:recommended"
        "extends": "airbnb"                 //popular eslintrc files
        //  npm command to install airbnb: npx install-peerdeps --dev eslint-config-airbnb
        //  npx eslint bad-code.js