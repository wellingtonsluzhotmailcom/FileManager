# FileManager
library to export internal jar files and copy files to different directories

 <h2>Export a file contained within .jar to an external directory</h2>
 <pre>
    File destino = new File("d:\logo.png");
    InputStream origem = Db.class.getResourceAsStream("/br/com/sisdespesas/files/logo.png");
    FileManager.exportInternalFile(origem, destino);
 </pre>
 
<h2>Copy a file from one directory to another</h2> 
 
 <pre>
   File arquivoOrigem = new File("d:\logo.png");
   File arquivoDestino = new File("c:\logo.png");
   FileManager.copyFile(arquivoOrigem, arquivoDestino);
 </pre>
