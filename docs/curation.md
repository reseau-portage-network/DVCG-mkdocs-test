# CURATION Steps

Step     | Description
---------| -------------
**C**    | [Check](#Check)
**U**    | [Understand](#Understand)
**R**    | [Recommend](#Recommend)
**A**    | [Augment](#Augment)
**T**    | [Transform](#Transform)
**I**    | [Include](#Include)
**O**    | [Optimize](#Optimize)
**N**    | [Note Down](#Note-down)

## Check


## Understand

In the Understand step, you should ensure the dataset is well-described and that end users will have a clear picture of what the data is and how it can be used. Review the metadata and documentation for thoroughness and clarity, create or recommend additional documentation if required, and check for usability issues such as missing data, code execution failures, ambiguous headings, and data presentation concerns. You may also screen for disclosure risk, intellectual property rights infringements, and other tasks, dependent on your institution’s policies and the level of curation service your repository provides.

For a thorough overview of steps you might take to understand the data and assess its completeness and usability, see Johnston (2017, Step 3.0). The Data Curation Network’s Data Curation Primers (2019) are another excellent resource with guidance and best practice advice for curating specific file types. They include information about tools for file review and specify information that will be necessary to ensure the usability of the data over time. 

### Level 2

#### Supporting documentation is thorough, accurate, and complete

If the dataset has a Readme file, codebook, user manuals or other documentation, review it for accuracy and completeness. The documentation should provide contextual information about the dataset to increase its usability. If documentation is inadequate, work with the researcher to enhance existing documentation, or provide them with templates and other guidance to create documentation. Cornell University’s “Guide to writing “readme” style metadata” (n.d.) and University of British Columbia’s “Creating a README for your Dataset: Quick Guide” (Brigham 2020) are useful resources for both curators and researchers.


Yes| No| Some Issue| N/A| Documentation includes a list of files...
----| ---|------------|-----|-------------------------------------------
&#9744;|&#9744;|&#9744;|&#9744;| Contextual information about the data (how the data was collected or generated, the goal of the research).
&#9744;|&#9744;|&#9744;|&#9744;| Description of file naming conventions and the structure of the files, if important.
&#9744;|&#9744;|&#9744;|&#9744;| Record of how the data were modified or processed.
&#9744;|&#9744;|&#9744;|&#9744;| Information about confidentiality and any restrictions placed on secondary use.
&#9744;|&#9744;|&#9744;|&#9744;| Names of labels and variables, information about allowable values and units of measure, codes and classifications, if applicable.
&#9744;|&#9744;|&#9744;|&#9744;| Explanations of codes and classifications.
&#9744;|&#9744;|&#9744;|&#9744;| Description of the computing environment required to run any code that has been included (operating system, software packages and dependencies).


#### Files open properly and contents appear as expected

Download the dataset and extract the contents of any archive file types (.zip, .tar, etc.). Review file content and address any issues with proprietary files. Tip: For unfamiliar file types, does the documentation provide guidance on what software was used to generate the file, or how it might be viewed? Try opening the file in a text editor as even binary files may have plain text headers with information about the instrument or software that generated the file. 

If it is not feasible to open all files, check a subset that contains:

- At least one of every file type in the submitted dataset,
- Script files, code, and anything you suspect may be licensed,
- Any file you have reason to believe may include sensitive information. 



Yes| No| Some Issue| N/A| .
----| ---|------------|-----|-------------------------------------------
&#9744;|&#9744;|&#9744;|&#9744;| Files open as expected and archive file formats extract without issue (unknown software, incompatible versions, or no access to the software could be a reason for files not running). 
&#9744;|&#9744;|&#9744;|&#9744;| If the files are not accessible, has the researcher provided a non-proprietary version of the files? 
&#9744;|&#9744;|&#9744;|&#9744;| If non-proprietary files cannot be provided, does the Readme describe how the data were generated, and the software necessary to use the data?
&#9744;|&#9744;|&#9744;|&#9744;| File contents are consistent with expected structure and encoding.
&#9744;|&#9744;|&#9744;|&#9744;| Readme file describes the data files and includes the following:<br>&#9744; Summary description<br>&#9744; File formats (flagged if proprietary)<br>&#9744; File size<br>&#9744; Path and/or tree structure<br>&#9744; Hash (MD5)


#### Files and folders are named and structured appropriately 

Ideally, files should be named and organized in a manner that is understandable and allows end users to easily navigate the contents of the dataset. The directory structure should be simple and directory names should clearly communicate their contents. The criteria below, provided by the University of Victoria (Khair 2020), are general best practices, and conventions for specific data types or discipline may differ. 


Yes| No| Some Issue| N/A| .
----| ---|------------|-----|-------------------------------------------
&#9744;|&#9744;|&#9744;|&#9744;| Filenames are free of spaces or special characters and use underscores or hyphens as delimiters (e.g., Datacollection_20201009_v02.csv).
&#9744;|&#9744;|&#9744;|&#9744;| File and directory names are concise, consistent, and understandable.
&#9744;|&#9744;|&#9744;|&#9744;| Dates in filenames use consistent formatting (e.g., YYYYMMDD).
&#9744;|&#9744;|&#9744;|&#9744;| Filenames use leading zeros for version numbers (e.g., v_012).
&#9744;|&#9744;|&#9744;|&#9744;| Files are grouped in a logical folder structure and are not overly nested. Note: Folder structure may be dependent on the code, syntax, or output of a piece of software. 

### Level 3

#### Code is well commented and produces the expected results 

The researcher may have included script files that were used to process or analyze the data, code that extends an existing model, executable files, or other software. While it may be beneficial to keep script files with the data, there are many purpose-built repository options for code and software that have robust version control systems and allow for ongoing development. You may suggest an alternate solution for publishing and archiving software and/or review the code and associated documentation alongside the data deposit. 


Yes| No| Some Issue| N/A| If the dataset includes software or code...
----| ---|------------|-----|-------------------------------------------
&#9744;|&#9744;|&#9744;|&#9744;| Is the code also available in GitLab, GitHub, Bitbucket, or another purpose-built repository?<br> - If yes, consider asking the researcher to archive it in the Software Heritage archive and link to it from the dataset metadata record.<br> - If no, and the researcher has included more than data processing or analysis scripts (such as .r, .m, or .do files), consider suggesting a purpose-built repository.
&#9744;|&#9744;|&#9744;|&#9744;| Is the code (or part of the code) derived from another source?
&#9744;|&#9744;|&#9744;|&#9744;| If the code is derived from another source, does the original source code allow for redistribution? Is the license compatible with the license of the original source?
&#9744;|&#9744;|&#9744;|&#9744;| If an executable file is included, is the source code also available?
&#9744;|&#9744;|&#9744;|&#9744;| Code is well commented<br>&#9744; The code contains header information such as: author, version number, filename, license<br>&#9744; The function or purpose of the code is clear (from the Readme and/or embedded description)<br>&#9744; If applicable, the depositor included information about how to run the code<br>&#9744; The required software packages and dependencies are listed<br>&#9744; Comments are concise and clear and describe the intention of the line(s) of code that follow, and/or the code itself is expressive (can be understood by humans and machines)
&#9744;|&#9744;|&#9744;|&#9744;| The Readme or a header in the code itself includes information about:<br>&#9744; The license<br>&#9744; The developer’s name and contact information<br>&#9744; The version, and the date the code was last modified and/or run<br>&#9744; Any sources the code (or part of the code) was derived from<br>&#9744; Instructions on how to install or use the code. If there are multiple scripts, the order in which they are run should be clear<br>&#9744; Required software packages and dependencies<br>&#9744; Information about the environment in which the code was developed and/or can be used<br>&#9744; Information about required input and expected output

#### Submission contains potential sensitivities

Note: Most instances of Dataverse allow researchers to restrict access to datasets, either temporarily or in perpetuity; however, Dataverse is not an enclave suitable for sensitive data. Review your Dataverse policies and/or consult with your administrator to confirm what types of information are suitable for your Dataverse ... **NEED TO COMPLETE THIS SECTION**

Yes| No| Some Issue| N/A| .
----| ---|------------|-----|-------------------------------------------
&#9744;|&#9744;|&#9744;|&#9744;| 
&#9744;|&#9744;|&#9744;|&#9744;| 
&#9744;|&#9744;|&#9744;|&#9744;| 
&#9744;|&#9744;|&#9744;|&#9744;| 
&#9744;|&#9744;|&#9744;|&#9744;| 



#### Submission contains data or code from third party sources

Datasets should be inspected for data or code from third-party sources to verify that researchers have the proper rights or permissions to share data, and that proper attribution has been provided. Although resources may be free to access, view, or use it does not necessarily follow that they are free to redistribute. Consult with your copyright office or specialists on your campus to determine how your organization’s policies regarding third-party intellectual property and rights affect deposit into your repositories.

Yes| No| Some Issue| N/A| .
----| ---|------------|-----|-------------------------------------------
&#9744;|&#9744;|&#9744;|&#9744;| Dataset contains proprietary or restricted information. **Example:** commercially licensed or proprietary data or code, or third-party data that are only accessible by registering or logging in.
&#9744;|&#9744;|&#9744;|&#9744;| Third-party data or code has been properly cited and the original terms of use allow for redistribution.
&#9744;|&#9744;|&#9744;|&#9744;| A data sharing agreement is referenced or included and allows for information to be redistributed.


## Recommend

## Augment

## Transform

## Include

## Optimize

## Note Down
