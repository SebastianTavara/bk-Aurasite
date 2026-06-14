# bk-Aurasite

### Download aurasite file
<br>
<img width="920" height="370" alt="image" src="https://github.com/user-attachments/assets/d55f5e4a-541a-4126-8c3a-1da7d01aba36" />
<br>
<hr>
### After that, type the following command:
docker cp <file address> <name of container>:/aurasite

<br>
<img width="757" height="39" alt="image" src="https://github.com/user-attachments/assets/ad19d96c-5ae1-4591-b060-5c3360f092f3" />
<br>
<hr>
### Now, inside the container you should see the aurasite folder:
docker exec -it db sh<br>
#ls /

<br>
<img width="1448" height="96" alt="image" src="https://github.com/user-attachments/assets/c1d6e5e9-c0b4-4e09-84d3-2584ec86168e" />
<br>

### Type the following command: mongorestore --db aurasite /aurasite
You should see something like this:
<img width="1499" height="399" alt="image" src="https://github.com/user-attachments/assets/6c413958-9059-4ff8-a6d9-01e3e393dd96" />

<hr>

### And that's it, you would now have the database in the Docker container

<img width="1516" height="456" alt="image" src="https://github.com/user-attachments/assets/5190e33a-da13-438f-a048-8aae77de57da" />


