# UEB-Testsuite
Student created test suite to validate implementation for the Ubersetzerbau UE in 2023S.

[Link to the previous year's test suite](https://github.com/flofriday/UEB-Testsuite)

## Usage
1. `git clone git@github.com:RFJBraunstingl/UEB-Testsuite-2023S.git ~/test`
2. The tests starting from the "scanner" example should be picked up automatically the the test scripts on the server

    optional
3. add following code to .bashrc
    ```
    function test(){
        pwd=$(pwd)
        basename=$(basename $pwd)
        git -C ~/test pull && /usr/ftp/pub/ubvl/test/$basename/test
    }
    ````
4. run ```$ test``` from dir you want to test

## Notes
- If you write your own tests, please share them by creating a Pull Request
- If you choose to do so, please prefix your tests with some handle (e.g. your username) to avoid conflicts
