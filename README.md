# MongoDB-Note

- client = MongoClient('url') 將 client 連線到 MongoDB
- db = client.pythondb 將 db 連到 pythondb 這一個 database
- client.list_database_names() 取得當前該帳號的所有 database 的名稱
- data_base_name.list_collection_names() 取得該 database 內的所有集合名稱
- ouo = client["pythondb"]["discord_user_data"] 可以使用陣列的方式取代 client.database_name
- for i in ouo.find():  遍歷這一個集合內的所有數據
- query = { 'type_name': 'old_data'} , new_data = {'$set': {'type_name': 'update_data'} } 更新資料
- update_many( query,new_data ) , update_one( query,new_data )
