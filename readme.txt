1.eslint:

    commands:
        npx eslint bad-code.js
        npx eslint bad-code.js --fix

    .eslintrc:
        "rules":{
            no-console: 0
            any-error-can-go-here: (values are 0,1,2)
        }
        //here 0 is off; 1 is warn; 2 is error 

        "extends": "eslint:recommended"
        "extends": "airbnb"                 //popular eslintrc files
        //  command to install airbnb: npx install-peerdeps --dev eslint-config-airbnb
        //  npx eslint bad-code.js
        //  to isntal airbnb globally:npm i eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react -g

2.git
    .gitignore:
        node_modules/*
        file.txt
        *.txt
        video*
        #comment
