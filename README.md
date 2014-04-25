# Dependencies
On Ubuntu, the python twitter library used in this particular package (i.e. `import twitter`) is [**Python Twitter Tools**](https://github.com/sixohsix/twitter) by @sixohsix.  
**NOTE:**  
* This is NOT the same as the apt-get `python-twitter`, nor is it the same as the rosdistro/rosdep 'twitter'.
* The website for the library is: http://mike.verdone.ca/twitter/
* The source can be found at: https://github.com/sixohsix/twitter
* The library is listed on the main Twitter developer's site at: https://dev.twitter.com/docs/twitter-libraries

# Setup

## Installation
These instructions assume you are using a catkin workspace, which already has your Baxter SDK `sdk-examples` repo checked out in the src/ directory.

1.  Install the Python-only module dependency (before sourcing any catkin_ws).  
    Install dependencies (Python Twitter Tools)
    ```bash
    $ sudo easy_install twitter
    ```

2.  Clone this package into your catkin workspace
    ```bash
    $ cd ~/catkin_ws/
    $ . devel/setup.bash
    $ cd src/
    $ git clone git@github.com:osrf/baxter_tweet_face.git
    $ cd ../
    $ catkin_make --force_cmake
    ```

