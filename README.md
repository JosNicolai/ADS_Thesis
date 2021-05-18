# ADS_Thesis

## The following files have to be downloaded seperately

iBabs20210415.tgz   -   Has to be extracted manually in order to retrieve all meetings.

Documents folder    -   Has to be downloaded manually with the Downloading Documents notebook.

DocumentsTexts.csv        -   This file contains the text from every document, which were converted from PDFs. Read with pandas. Download from https://drive.google.com/file/d/1ZlZzmcF5kk2HmMy1m7It8SRFBQ33yBKm/view?usp=sharing

shortest_paths.csv    -   A file containing the shortest paths between every item/agenda point. Download from https://drive.google.com/file/d/1bxAumfMJE2LEkb1NoTtQTrwrLNNs7xdr/view?usp=sharing and read with pandas.


# Beneath here is outdated, will update soon.


## ProcessedMeetings directory

documentsInformation.txt  -   A file containing information on all documents with the same ID. To read use pickle.
itemsInformation.txt      -   A file containing information on all items (agenda points) with the same ID. To read use pickle.
meetingsInformation.txt   -   A file containing information on all meetings with the same ID. To read use pickle.

nonDuplicateDocumentsInformation.txt  - This file consists of all documents from documentsInformation.txt, but every document 
                                        with the same title has been filtered. To read use pickle.
                                        
Document_item_match.csv   -   This file contains every document and the items they are connected to. Read with pandas.

## The following files contain the code:


Retrieving Meeting information.ipynb    -   This notebook file contains the code to convert the xml files to the above txt files. 
                                            For now contains code for the creation of a network.
   
PDF-To_text.Rmd     -   R markdown file containing the fastest way to convert the PDFs to text (around 2 hours of processing).
PDF_to_text.ipynb   -   A notebook file containing code for converting all PDFs to text, looked best, but very slow (~30 hours).

texts_to_csv.ipynb  -   A notebook file which converts all seperate text files to a pandas dataframe.

Downloading Documents.ipynb   -   A notebook file to download all documents using information from either 
                                  nonDuplicateDocumentsInformation.txt or documentsInformation.txt.
