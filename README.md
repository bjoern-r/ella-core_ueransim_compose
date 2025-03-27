# ella-core end-to-end with UERANSIM docker

 - ip settings are in `.env`
 - `run docker compose up`
 - navigate to http://127.0.0.1:5002
   - add a user
   - login
   - change operator -> OP to `11111111111111111111111111111111`
   - add subscriber
     MSIN: `1234567895`
     Ki: `8baf473f2f8fd09487cccbd7097c6862`
 - restart docker compose
 - test datapath in UE container
   - `docker exec -it nr_ue ping -I uesimtun0 8.8.8.8 -c2`