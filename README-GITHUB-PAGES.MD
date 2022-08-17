
README.MD for 
https://github.com/txtjqm/txtjqm.github.io

It hosts the knob react app on github.

see page at:
https://txtjqm.github.io/TestReactKnobInGrid_url

It was made this way:
* edit ~/.ssh/config to add entry for new ssh key
* add new ssh key using above name...       ssh-keygen -t rsa 
* on github console add "deploy key" and copy/paste id_rsaZZZ.pub [the public]
  key into it. THEN CHECK READ/WRITE CHECKBOX!!!!
* logout/in to let new ssh-config file to take effect and get the project:
* git clone git@host_rsaGITPAGEZZZZZ:txtjqm/txtjqm.github.io.git
* cd txtjqm.github.io/
-- phase 2:
* in project where react project is run...    npm run-script build
* copy all files in newly created "build" folder into top level of
  local folder above, at its root level.
* git add .; git commit -m "new react project"; git push;
* browse to.....      https://txtjqm.github.io/TestReactKnobInGrid_url

*** important note: need to make node path relative so above 
    [non root level] link above will work.
* in package.json add line "homepage" as below:
...
  "name": "react_app_123",
  "version": "0.1.0",
  "zz": "added toallow relative path for modules instead of / for github pages",
  "homepage": "./", 
...

