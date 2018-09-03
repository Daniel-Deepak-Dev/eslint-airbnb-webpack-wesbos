# ESLINT

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
            //  to install airbnb globally:npm i eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react -g

        "plugins": ["html"] // to use this plugin should install it first
            // to install above plugin: npm i -D eslint-plugin-html; so that every html can be linted by eslint
    
    eslint comment functions:
        /* globals twttr ga*/ to ignore global varibale errors
        /* eslint-disable any-error-or-warning*/ to disable errors below this comment use enable keyword to enable it
        /* eslint-disable*/ will disable entire eslint package for the codes below it

#git:
    .gitignore:
        node_modules/*
        file.txt
        *.txt
        video*
        #comment
    
    can tell git to commit only if code passes all eslint errors by wes bos git commit-msg file in
    - .git/hooks/commit-msg-sample rename it to commit-msg
    - then add/replace the lines from git commit-msg file.txt in this repo
    - now every branch-user who want to commit must follow the eslintrc rules 

#babel:
    npm install babel-loader babel-core babel-present-es2015-native-modules --save-dev
