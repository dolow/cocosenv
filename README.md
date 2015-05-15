# cocosenv

cocosenv is the light command file to wrap cocos command and let this run in any desired version.

## Usage

1. put cocos2d-x versions in the same directory and leave their name as default (name with prefix "cocos2d-x-"). Otherwise, $COCOS_PREFIX variable must be defined as prefix.

```
export COCOS_VERSIONS_DIR=/Users/kuwabara_yuki/lib/

# configure this if you have changed the name
#export COCOS_PREFIX="my_prefix_"
```

2. define the directory as $COCOS\_VERSIONS\_DIR

3. put cocosenv file to any directory you like which is referenced in $PATH, like /usr/local/bin/

4. use cocosenv with version name, version name is a part of cocos2d-x directory name after the prefix.

e.g.
```
cocosenv 3.4 run -p android -m release --ap android-14
```

### Options

| Option       | Description                                  |
| ------------ | -------------------------------------------- |
| -l           | list all available versions                  |
| [version] -p | displays path to cocos2d-x version directory |


### Notice

This command is tested with cocos2d-x 3.x. (includes 3.0 beta, 3.0 RC)

cocos2d-x 2.x is not supported.
