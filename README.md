# commands

#Transfer file from local to server (-r to transfer directory)
scp local_filename.txt name@xxx.xxx.xxx.xxx:path_to_insert 

#Transfer file from server to local (-r to transfer directory)
scp name@xxx.xxx.xxx.xxx:path_to_get/filename.txt ~/local_path_to_insert 

#Get mongo find query output into a file
mongo --quiet dbname --eval 'printjson(db.collection.find().toArray())' > output.json

#Insert json file into mongodb collection
mongoimport --jsonArray --db db_name --collection collection_name --file file_name
