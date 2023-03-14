###  Data description

1. /main/QoS.json 

   Collection of QoS evaluation indicators;

   The sample of data format:

   ```json
   {
   	"index": "XX",
   	"name": "XX",
   	"description": "XX"
   }
   ```

2. /main/QoE.json

   Collection of QoS evaluation indicators;

   The sample of data format:

   ```json
   {
   	"index": "XX",
   	"name": "XX",
       "category": "XX",
   	"description": "XX"
   }
   ```

3. /main/QoE_Embedding_vectors.csv

   Representation vectors of user personalization preference;

   Data shape: (65878, 64).

4. /main/Weights_W.csv and /main/Weights_b.csv

   Parameters W and b of user satisfaction mapping functions;

   Data shape: (65878, 69).

5. /main/UPP_Interval.csv

   Preference range of each user for each QoS attribute;

   Data shape: (65878, 69).

6. /main/UPP_Direction.csv

   Preference direction of each user for each QoS attribute;

   Data shape: (65878, 69).

7. /main/SDQ_hotels.csv

   Normalized QoS of hotel resources;

   Data shape: (1236, 61).

8. /main/SDQ_rooms.csv

   Normalized QoS of room resources, associated with the file "/main/SDQ_hotels.csv" via hotel ID;

   Data shape: (5064, 11).

9. /main/model.pkl

   The model instance of initial multi-level SLA customization by granular computing.

10. /main/model_matching/*

    After accurate matching, the granular structure is unchanged, and the subset of users matched by each customized solution at layer i is shown in the table "layer_num_i.csv", where "**True**" indicates that the user matches the current customized solution. 

11. /main/model_reduction/*

    Results of model reductions under different parameter settings.



Since GitHub does not allow uploading files larger than 100M, large files are compressed, and the name of the compressed package is the same as the original file name above.

**Other questions, please contact: limin19961996@163.com.**
