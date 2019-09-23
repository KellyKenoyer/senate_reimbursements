# senate_reimbursements
#This is a project that takes pdfs, converts them into readable text files, then turns those into usable csv files.
#The "get_all_headers.py" file has some interesting code related to analysis after the data has been cleaned. It created a file list with the command file_list = [various files], then created a command for the entire set of files in file_list, to open it with csv.reader and pull the first_row to line[0] and copy it one over (unless there's an error). Essentially it pulls data from a large number of files, puts them all in one place, and then prints the newly organized information. It's also doing something with "keys", but I'm not sure what that's related to.
#Here's the code:

#office_dict = {}

#for filename in file_list:
#    reader = csv.reader(open(filename, 'r'))
#    for line in reader:
#        first_row = line[0]
#        try:
#            office_dict[first_row] = office_dict[first_row] + 1
#        except KeyError:
#            office_dict[first_row] = 1
#
#
#writer = csv.writer(open("headerlist.csv", 'w'))
#for key in office_dict.keys():
#   print "%s - %s" % (key, office_dict[key])
#   writer.writerow([key, office_dict[key]])
            

