# bk-Aurasite

## Restore AuraSite Database in Docker

---

## 1. Download the Backup File

Download the **aurasite** backup folder.

<br>

<img width="920" height="370" alt="Download backup" src="https://github.com/user-attachments/assets/d55f5e4a-541a-4126-8c3a-1da7d01aba36" />

---

## 2. Copy the Backup into the Container

Run the following command:

```bash
docker cp <file-path> <container-name>:/aurasite
```

Example:

<img width="757" height="39" alt="docker cp command" src="https://github.com/user-attachments/assets/ad19d96c-5ae1-4591-b060-5c3360f092f3" />

---

## 3. Access the Container

Open a shell inside the MongoDB container:

```bash
docker exec -it db sh
```

Verify that the backup folder exists:

```bash
ls /
```

You should see the `aurasite` directory listed.

<br>

<img width="1448" height="96" alt="aurasite folder" src="https://github.com/user-attachments/assets/c1d6e5e9-c0b4-4e09-84d3-2584ec86168e" />

---

## 4. Restore the Database

Execute the following command:

```bash
mongorestore --db aurasite /aurasite
```

Expected output:

<br>

<img width="1499" height="399" alt="mongorestore output" src="https://github.com/user-attachments/assets/6c413958-9059-4ff8-a6d9-01e3e393dd96" />

---

## 5. Verify the Restoration

If the process finishes successfully, the database should now be available inside the Docker container.

<br>

<img width="1516" height="456" alt="database restored" src="https://github.com/user-attachments/assets/5190e33a-da13-438f-a048-8aae77de57da" />

---

**Database restoration completed successfully.**
