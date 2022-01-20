# GETとPOST分ける
## 試す
flaskでgetとpostを分けたいなら簡単で、routeのところを
methodsつければいい。

かつrequestで取れる。入れるのは`pip3 install requests`とかでいい

    from flask import Flask,request
    app = Flask(__name__)
    
    @app.route('/',methods=['GET','POST'])
    def hello():
      name = "Hello World["+request.method+"]"
      return name
    
    if __name__ == "__main__":
      app.run()

POSTを打ち込むのは`curl -XPOST -d '' "http://127.0.0.1:5000"`とかでいい

## 他色々参考
https://qiita.com/aKuad/items/400550b76d79c0d2cd3c
