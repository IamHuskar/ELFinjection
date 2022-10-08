# ELFinjection
ELFinjection is a simple utility for inject so, it can do the following:

* Using ptrace to inject a so file into the process
  ```
  ./ELFinjection -p  <pid>  <libpath> 
  ```
* Use ptrace to inject a so file into the process and execute a remote function
  ```
  ./ELFinjection -p  <pid>  <libpath>  <funcname>
  ```
* Add a declared dependency on a dynamic library (DT_NEEDED)
  ```
  ./ELFinjection -e  <elf_path>  <so_path>
  ```