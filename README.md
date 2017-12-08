# mmmstudio
Minimal components of mmstudio (Micro-Manager) to allow read/write of the image data without GUI

Sometimes you need to operate on micro-manager data outside the GUI program. You can do this by referencing
MMJ_.jar and MMCoreJ.jar in your own JAVA code. However, these libraries was designed with a GUI in mind and 
won't run in a headless environment (e.g. a HPC cluster). This small lib strips all classes that are not 
necessary for read/write of micro-manager files and removed all reference to GUI functions.
