# Python-Util-pickleShow
This Casspop Codelette monitors changes in pickle files OR shows contents of selected pickle files.

Put pickleShow.py in the folder where your pickle files are located and then invoke it from the command line:

<code>greg@brilliant:~/all$ ./pickleShow.py</code>

With no command line arguments, pickleShow.py will display the Unix Epoch Time value for the last time each .pkl file was modified. Then it will monitor the status of those values, and when one of them changes, it will display the contents of the .pkl file.

The point of this is to give you a clear understanding of when your program writes to a .pkl file, and what it was that was written.

When you use the -s command line argument like this: 

<code>greg@brilliant:~/all$ ./pickleShow.py -s</code>

pickleShow.py gathers some stats and then:

- tells you how many files are in your working directory
- tells you how many of those files are .pkl files
- iterates through the list of .pkl files asking you if you want to see its contents
- waits for you to respond (y)es, (N)o default, or (q)uit

If you press "Enter", the (N)o default passes you on to the next file.  'q' (Q)uits back to the prompt.

'y' will display the filename, the type of the pickle file, and then the contents of that file.



