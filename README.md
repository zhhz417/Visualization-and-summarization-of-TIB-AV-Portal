# Visualization-and-summarization-of-TIB-AV-Portal


All this dataset is about the German-videos which have ASR results.


----------


 - **Files**
    - **german_gndID.csv** : all IDs of GND for each German-video. 
   Two columns [videoID, gndID]
    - **german_gndLinks.csv** : all links of GND for each German-video. 
    Two columns [videoID, gndLinks]
    - **german_gnds.csv** : all GND's names for each German-video.
    Two columns [videoID, gnds]
    - **videoResources_complete.csv** : the links of video resource, video urls and the languages for each German-video. 
    Three columns [videoResource, videoUrl, lang]


----------


 - **Transcripts**
    - Folder 'german': all raw speech transcripts of German-videos.
    - Folder 'english': all raw speech transcripts of English-videos, which have ASR results.
    - Folder 'de_timestamps_raw': all raw speech transcripts of German-videos with timestamps.
    - Folder 'de_timestamps_Tag': all speech transcripts of German-videos with timestamps and POS Tagging.
    - Folder 'keyphraseTable_ordered' : extracted keyphrases with timestamps.
    


----------


 - **Codes**
    - **portal_Metadata.py** : parse RDF file, return metadata of required video and store them as a csv file.
    - **getContent.py** : crawl transcript without timestamps.
    - **Content_timestamps.py** : crawl transcript with timestamps.
    - **data_preprocessing_TS.py** : preprocess the transcripts with timestamps.
    - **keyphrasesPKE.py** : extract keyphrases using pke.
    - **visualization.py** : embed entities into the vector space and reduce the dimension.
    - **plotly_Visualization.html** : visualize the entities using Plotly.


