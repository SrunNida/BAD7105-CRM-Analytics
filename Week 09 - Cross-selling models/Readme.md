# Market basket analysis

First, import data from survay file

![image](https://user-images.githubusercontent.com/88968324/146056864-0b766a39-fb99-4b28-8b56-fd780176d838.png)

As we can see, every columns has null data

![image](https://user-images.githubusercontent.com/88968324/146057016-50207aae-8c00-4fff-b20b-0752e7deac8e.png)

Preprocess data by
- Fill in null
- Replace some kind of word 'not' to 0 and else 1

![image](https://user-images.githubusercontent.com/88968324/146057284-56e62b27-a52d-4a14-a489-24f75802f21b.png)

Count and see top 10

![image](https://user-images.githubusercontent.com/88968324/146057411-4ead3de2-56cf-43d0-8cc7-8ea7c7685d62.png)
![image](https://user-images.githubusercontent.com/88968324/146057435-f7c049b9-7d2a-4b4a-9757-dbcae232509d.png)

Find frequent item set

![image](https://user-images.githubusercontent.com/88968324/146057568-98c4ab2b-93c8-4ffd-8943-be9d246a91bf.png)

Decide on Support threshold

![image](https://user-images.githubusercontent.com/88968324/146057637-a453654a-10bb-4641-99c0-29d6997c69fc.png)

Top rule based on 'Confidence' score

![image](https://user-images.githubusercontent.com/88968324/146057717-1b4d5da2-3c79-4fcd-a6af-e004a3fb9271.png)

Top rule based on 'Lift' score

![image](https://user-images.githubusercontent.com/88968324/146057777-f4bf64d6-1614-4c68-90fc-2e251d055f2d.png)
