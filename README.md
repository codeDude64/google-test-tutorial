# Cmake and google-test set up

I'm follow the tutorial https://raymii.org/s/tutorials/Cpp_project_setup_with_cmake_and_unit_tests.html 

## Command to running (for the moment)

just like the tutorial mentioned to build the project we need to (go/create) the build directory and run 

`cmake .. -DCMAKE_BUILD_TYPE=Debug -G "Unix Makefiles"`

then in we should still on the build directory, run the following command, in order to make the execs file.

`make all`


If you are using neovim and lspconfig with ccls (just like me) then you should run the following command on the build directory

`cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON .`

This command gonna create the compile_commands.json on the build directory.
With this json file your lsp server gonna works as expected on your project.

