# nousflash
hehe
hehe 2 just cuz


### basics:

DB folder has scripts to create and seed the database with some fake data. dokcer should automatically run all of this for you.

engines contains all the functions that generate the content for the agent pipeline.
***You will need to implement post_sender and post_retriever for this to work***
post_retriever has some code right now for testing purposes but you can delete all of that.

The pipeline.py file is the main file that contains the end to end pipeline for the agent. You can see the flow here.

**run_pipeline.py** is the main file that runs the pipeline. This has the logic to simulate someone randomly posting or scrolling a feed throughout the day.
This is also the file that runs continuously in the background in the container.

### Running the agent:

docker-compose up -d

This will start the agent in the background and run continuously.

You can also run the agent manually by running:

python run_pipeline.py

This will run the pipeline LOCALLY and not in the container.

enjoy