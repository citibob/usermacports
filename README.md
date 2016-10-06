# Instructions

1. Download latest MacPorts srce (.tar.gz version) to ~/Downloads: https://www.macports.org/install.php#source

2. Edit the file new_macports.  Set the variable MACPORTS_DOWNLOAD to the name of the file just downloaded:
    ```
    MACPORTS_DOWNLOAD='MacPorts-2.3.4.tar.gz'
    ```

3. Run the ```new_macports``` script to create a new user-level installation of MacPorts, in a particular location.  For example:
    ```
    new_macports $HOME/macports/gcc49-python3
    ```

4. Set up your environment in your .profile:
    ```
    export MACPORTS=$HOME/macports/gcc49-python3
    export PORT=$MACPORTS/bin/port
    export PATH=$MACPORTS/bin:$PATH
    ```

5. Install stuff in your new Macports directory; just use `port
   install` without the `sudo`.
