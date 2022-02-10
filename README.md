# milestone135N
The purpose of this assignment is an introduction to loading and saving data from an application to text file.

	
  
  At this point the entire console application is working with all the main menu items performing their action.
	When you start the application, it will look for a data file that has serialized objects and deserialize to build List<BaseContact>. 
  If the file does not exist or the file is empty, then address book (List<BaseContact>) will start off empty.
  If you have contacts from a previous run through, it will load before displaying any menu.
	When you select exit from the menu, all objects in List<BaseContact> will be serialized and written to a file. 
  This file will persist even after the console application closes. 
## Structure of Application
1.	Base Contact – Abstract class containing information common to a personal contact and business contact. Properties include contact id, name, phone, list of photos, and location.
2.	Person Contact – Properties unique to a person include date of birth, description.
3.	Business Contact – Properties unique to a business include business hours and website URL.
4.	Location – A class that contains geographic location data including location id, street name and number, city, and state.
5.	Photo – A class that contains information about a picture. Properties include photo id, file name, date of photo, and description.
6.	AddressBook – Contains list of all Contacts objects in the app. Methods are needed to add, remove, update, display one, display all, sort by name, and search for contacts by name.
7.	ConsoleApp – Has a main() method that create instances of the other.
8.	DataAccessService – This class will have methods to readAllContacts and saveAllContacts. 
