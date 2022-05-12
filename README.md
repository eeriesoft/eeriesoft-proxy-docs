# eeriesoft-proxy-docs


1. Get the dcom . list

    URL: [host]:[port]/api/v1/dongles/all
    Method: GET

2. Change ip by port

    URL: [host]:[port]/reset?proxy=[proxy port]
    Method: GET | POST
    Example: http://192.168.10.111:6868/reset?proxy=4000

3. Change ip according to proxy

    URL: [host]:[port]/reset?proxy=[proxy ip:port]
    Method: GET/POST
    Example: http://192.168.10.111:6868/reset?proxy=192.168.10.111:4000

4. Change the ip of all dcom

    URL: [host]:[post]/reset_all
    Method: GET | POST
    Example: http://192.168.10.111:6868/reset_all

5. Check dcom . status

    URL: [host]:[post]/status?proxy=[proxy ip:port]
    Method: GET
    Example: http://192.168.10.111:6868/status?proxy=192.168.10.111:4000
    Response: {status: true} if dcom is ready
