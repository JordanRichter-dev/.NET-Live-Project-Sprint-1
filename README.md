# .NET-Live-Project

Personal Code Summary for the team live project I was a part of at Prosper IT Consulting



Introduction
------------


During my time at The Tech Academy, I was assigned to 2 two-week sprints working on software to be used as a way to "manage a collection of construction jobs. Admins will be able to create and distribute a weekly schedule assigning users to certain jobs. Users will be able to keep track of which job they are assigned to for the week. There will also be the ability for admins to post company news and announcements, and chat functionality for the users to socialize."

My contributions to this project included adding back-end search functionality to the database within different pages of the app. This involved displaying ActionResults to Views, and using Partial Views that shared information within different parts of the app.  I also worked extensively with user roles and authentication as well as error handling, UI/UX navbar improvements, and adding and deleting objects to and from multiple tables with the database.


Listed below are the stories I worked on, a brief description of their expectations, and the code I created to complete them.

## User Stories
* [Front End Stories](#front-end-stories)
* [States Dropdown](#states-dropdown)
* [Sorting, Paging, and Searching ](#sorting,-paging,-and-searching)
* [Admin Header Nav Bar](#admin-header-nav-bar)



###Front End Stories

Styled the Scheduling page:

![img](images/-tWnqFxFBNVbT7XBtC6bsm1ku7nAqkeHhDiwmyK3cSZyivnCJKCFCtjQpYO5Ih-oRHlqALKHUlws1l3xi7daOm_2nYh43q2f_zDusZlkCAJEorM6giyBbqJPgcdM3MEsuOAc2YuV-20191009115909377.png)

Allowed resizing for "Body" textbox:
Before:

![img](images/8n0seYD6La9Ts_NPJ-m8aJc2MwCL0S1JY2XZ4YpYFpwcB1aGzwzlpsuEfAZxNT8a-7gY25D8x3eXWoe8kiQPilANyG5GUiOW_fBRtC0Co1BVABrcvUvaUNwd8L7WqilO1Bl_dyZo-20191009115919748.png)

After:

![img](images/yMjibqanTJ6hqgktaD8j45s9lWg7iVERCLyT6yBB0RzGstmD7tDUnhKZWdWVBj-JFFIJZzMWjamsxH4S_NPdBc6ffWCnZKCbjhqtAEBSVbbYkrJLVzhCtp1Tct-Ylt8LS_qanFjb-20191009115933000.png)

On this story, I stylized the background and buttons using CSS:

![img](images/hj0NhhiZO6gCSMlhyUrgKXvc7DN6FLtx5lqgoPm5jEaTv9x2w-wd7v28vKQ7CnCL8pzUqGDiIlIsCMNWTTOCnBU1sh53RTtOi1Pp_iApXObrm1sSd-_z20CMTmwvrrTPTe3kPKay-20191009115938654.png)


Before:

![img](images/f0WsS9td5UVFk_yTU_RLKIKv6Spex9XY5lFfYI2HBYaCOxjR_48EUUxlDYdnj1D3sObZWflFCIUYxCP4aJ9Q2YAKrNWV-g1ztMzt4iIVc6tj4T_P7YibEsYckw0Pz5t5PPWJsngj-20191009115948105.png)


After:

![img](images/YonLs-AQ8Tpf1wwx9AWoOe0ralXbyhEurfKrZtYdUgt3n86zlNnhCH_T3h3Bmizt5M3gCVUd7aZZ8tGO9oUJnKEyZWWZmKBxSbVVlLPDKGTmwAcuI6oFaWUnBUS8cUnZJtdVl6pV-20191009115958364.png)



I also added a jquery reference for error handling:

![img](images/TEs06TvRFgCM3r5K8GZaF-9vOi9r3QYMwaFAsaTCMzUuPtOiA_i518UBDK0pEtF-ioCbh7mY-ezXWM5kb4F-cLxPyJ0zcb44RY5MxCkGdIJs_JMreZmKnGHaTOh87jJx7o1O5y6C-20191009120720037.png)



**<u>Full Stack</u>**

###States Dropdown

On another story I added a dropdown menu for selecting States:
Here are code snippets that I added:

In View, I added access to DropDownList:   

![Screenshot 2019-10-07 16.52.09](images/Screenshot%202019-10-07%2016.52.09.png)

In JobsitesController.cs:
![img](images/lYcf41YwoRQeo7YFQNw1uBFqvdYh611diQRJ9wjqnPep5hrh78q7p6dosQIVumPGoOx0elghietmoOH39XBumNW8z5b6_Eq9aXPVo1d2C-nu15-Ik7C6bsg10fCZJMggD19Ab_90.png)

Before:

![img](images/5J1An4VbZxuoW3MHAq_qcIDHzd92gkO37HJd5cgdJdgkmOAWY3JEwVBsd1sanCLIkf22sBq61QA5lU-G7PQweGnYDGehMJsQqFYXLX0JlJkwnJxK6F2-RT0ImGMLgPTvP9RRlFiL.png)




After:

![img](images/BnnHMqBf2NDBJ8FG4a0lp2HzEa15GUwGMwkWExjFwTJnXDzcsF3-mvN9VR2Nl3ZMhooeIzFIJfKGEKMjwLDh6OPexV6V_UuCkYQG_Yb82evWmtu5JSRxYwKGKONY_a_xINh0MKkS.png)



###Sorting, Paging, And Seaching

This story asks for items in a Form List to be sorted by date and alphabetical order, as well as order by active jobs or passive.  Also add the ability to search and page through as jobs are added and app is scaled up:
Finished page:

![img](images/796aclT9_QpZeQEJwWk_fk70MLZqLZquMYuAyhV78AL53-hMyn9uMkB2S8cHbjCAPjscExS-AGKa_6-kS2EtpsJEkVVhSbRRp5rzRJbSxL469MjuPYyHrA_oB7yW8VU5Eove5wBE.png)


Adds Order criteria -
In JobsController.cs:
       

![img](images/_z_4efa5tou4AzvRkdDNnwLFUHigbiOQOZJCC5DM_ojfGrjQPSZOxAwIqzuhe5AWn2875RBNCA9hMTL-m5zlerIBlPnrRnaZRNGrhk_oX8sVUhTy4Wf9IZUkzK4DbMoCQlFj9QXN.png)



Views/Index:

(clickable hyperlinks for changing order) 	



![img](images/DndQ7U5V-nDFWaATQvceFfdtwcXMB7D-APW7nmSwwoZhZynANuF_SO16NhxiK-K99HxEReuJlCWkuq0jHVd6-yeZiEyJYSWeLwRj2ONiu7Rncj1UPp-SQ4rwS4RXTeoBFRIUIWR4.png)



Adds Search Box:
In JobsController.cs:

![img](images/DBNYW7x1b5emsoW8EFGegweeKgFfDBuB4goMjAPhXLyEG8rQgAwHgSHjQVLqMmxsUgYT9q_Itn5EWonjTYIuEByeoRGCkZ1GuqEHRGFaJ6NG1ppp__8UOoDGwO47qCsX13KRIPzi.png)



Views/Index:

(added search box and "show jobs" button)

![img](images/goi76mxBojd-WvQP7PgoVqF407D22koxqvx1Yxg6Kvv8JXiEFqAcbR03fDEjHyPvCyl7t3aclCO7lX1mFkWrqfsKXwIIuZx3w3z7q5bfle5318cLXLq2Oe0E5Tzlo-xZIIBOosw6.png)





Adds Paging (installed NuGet PagedList.Mvc package)
In JobsController.cs:

![img](images/5UE9JGCQ_FyE5doDuQFyxL9Jh0kNNI6o23-P-Nu1MIhiFxnD8xLmqAWv711srWbgzzPAEb56GUPK7ozPHXMzEKSBUZo6aY0PYdqMNWun7Zo1D4Ei0E46H-wCExcRTXsOTI5YVcr-.png)





View:



![img](images/0y3bvfa75a3rKWWLZCZrGUhzPGdOS7b39zZtfQsnDoSV_x-iv4Yfk_hf32r0-CTwPbduSye-27MvqgN-ycMSzMiV6zGpN6PX-a4DJLMsBXg17_ODBNerDyJ00KBvaxXsrvLPg7KH.png)

![img](images/QNLh4hfqe3M6mOIpEYqXB3zZevQJd8x6ueAkD8VWeZlUYPUgbmH-q1xqs7yya9xGMrazn1jjdkTYyNSTtbFjKPAv_QPyQOw7ZTB8K8e_8yxYs9w0x0v0rZDtCa9iO3ksoE1pCcyo.png)



I did this for three different pages of the app.  Here is the Company News page:

Before:



![img](images/LsHtsy0l6tevF9-kMMaic1qOEytQC0FG7kXlMlvoO7TPcn1aH9GOgjX2EBt80oYuoDz_z-ElrctmOueJtKVY3jsJDf0MgUrpjePn4DPecnJIfiqXxOeGHx4cbhn0_eqJz_wkHUCv.png)





After:

![img](images/BgvG41_kbKPmjORSvDLEkI8QpRlwikbziXFoyig8myW7sF1zVWvT9TyE_5tatZnOcHrrIOfB_4TMkPB7-CG-eI1cArrX2Q2fhZl3efS0dOIxh2pIIsFhvvXmu0iklHaWsDPRSOOc.png)




Here is the same type of code with the Scheduling page:



Before:

![img](images/drYWzzR7nsoyxiGgokj0PnKws3DtgjAxif1f8Cvy8GUrG9FGj_6quF2rjLMccciBvwN_27zNgamFsiQHYv9pAobfhSCDHRBmXd0xVVn6UqhT-ndEeIdkiaexSRIxwx6QKLzhO4i9.png)





After:



![img](images/bI9efVWmKZ1g9vbLYpRIHDOr-C-IfN2GgX_Tn7-5pkp4Hf0daMNk4SWqGpXGOtwI5TVPrd5LsLlF2oHh8mjAt1F-t-iHIOZR7byofd7ygif-tP5vl-RboskEVr8W_cRZbI394wvU.png)





Here is some of the code for the Scheduling App.

Controller:

![img](images/VO2UQKH0cxXu4moSf-n8brSSDA0vGJRlKrsHdGWOmBNf257bTWfKLU69KR2QAvA1lSjKlTcvn-F5U0YhVjTiIAF3hZIfT5_MQ7O7FYaecX6tbFyhW2G8eRXjxXC-OT5jyQLRW_Mb.png)

![img](images/HJzpLZFtIyu4qQcdbFlqvEkUX2PSuSzERCdoGFFPuIZC5Y8I7QzMx7V8d9gWXF7TdbB5J0Qsn65t7ZaZfRZMdu27rxzCQ73qXv9uXQbtDnQyOLn0s4QKqTqvt-hbPBimCGPkThId.png)



View:

![img](images/AFxeGl7SGaLNgb8GxqW6cb7BOuD6_PMQsAyQArPlHaBdDvWmoIqEZweb26XRn1AchvSM55yDQF13dkiyg5MYot6O4ofSXZ0sT7S1BA7Ng93qWppQJZ4qWusKNpcaZ3VQBlUTMGYQ.png)

![img](images/WvrEoOQ-RVxZ-w6kE2xh0N5JWlyVz9rADxpn1k-GLcOm4bFHyIhTNlex01ePdBJTVn-DjBeShSP6d2YmLm6OwxrVIudqjMoslXgQ5LpofIZBnz-kpIaXrykY_sRDcVBRfVXJyzey.png)





###Admin Header Nav Bar

I added a Dropdown Navbar in the Header that appears only when logged in and displays user's name:



Before:

![img](images/wZAUhAnSbjIsx2TaSILHkq6xZVc2EbkB-wmV7cSsQO2CkJ-KVHL9FZYmwCp7ab5PcmaGwrT1y4skQaLyensw1XmjUv6w0YHpQSJvwAnR4oVzoysRZfqhDP9sHmueO2redkl1Fdar.png)



Partial Views:

_Layout:

![img](images/YMVthDQH6SdxcoZVjITddakWuD-rd-e411Z-823FsNLxT39595k02O3zbRtn4ccB86QBrbpt5VQ9dOxLjqYzyMGcahMi6jO0SKb8Q2dM8jjJNk-qoHv883DqIXy5BMm-n0fI76RK.png)





_LoginPartial:

![img](images/TOSbxGmKr1k0Blz6h26W9uahuv8YzIIio5GC2rC1mdBVhCIpFXsKoFnXXuDPZt7mEtj8uRsuw3C2y6oBKCftzJDi2VIYy6Usvi_H1VSEN4sPYPAhaHhv85j9DV6X2NCJ0aode7zP.png)





I added the following code to the controller and views to allow creation of Admin Role in the View:

![img](images/BiBtRND0MlYzdW_2tgSZ_Q7RGDjGTHKBJYUCRvqHNRRw1_zhcRV2JnSzLa4-P0sbaTYeVKaPQ-wldS0CXlpMRSSKnRMbb06uskFGLxW14WphPNiqM7KgmAKGSw-t7nFZgpQJvX-w.png)

CreateUserRequest/Index.cshtml:

![img](images/puXRef974Ilojh8U0FuTd5p7IR1kFbBJ9R0ay88Lb9oVVZt4owIv-r6NDWET0fNf7_hg_S-sU5FT5_OjKggMfHO1R1NiLw8o59F6z_RpVIla_Mm1dz6DWohPcyhhWO2PpOEa8Dyn.png)





Created Index view under Role:

![img](images/GA2srU8nuy8k6Ydthz2fDguP7OjYKseLCTBN_tPpoP587Zw4-Dd5XasIndD4lZsk6nfkaJpptqDN0YJvHWwoqc0yYqfpkAjqOxOU-VYvISVuhFxFchVhoIlXBfAebUaV_Gqfvz3R.png)



Here are some of the CSS code I used:

![img](images/pPGvScYki60v3XILI9Hw640gVg5n08dOi49yJyjFOOH45oLfwb5v0wmIH1eo4a5Hio9Q0gu9HefMvyoy4vyjSGpXcZ3u4d6LYEwSkAwK32RRWB3Xc4kS_amEHdQcNGnphgEQJdPY.png)

![img](images/3z7l0f01g56sCGs4QD21ceLTstMNWjZa-LKLLatEqieQozm9jFjcA5x_bOnUGh8HTC11tRa6kYYNFlZnclat0CN284e5EhPY4I4Ba_ojRf8sf-7L_iKy0LFdUTynKMfSV05LNUdd.png)





After:

![img](images/OnZvKCSSKJi-J-g9D1jl60VzQNRM7vZKkoruV10U7Abe2wG-EulvgIuWdDU-ljYpJnPobLk4ZiKrLPpLCHAB7tINYGP3jGNdgRqCRarGUC71v25z2NpPu_KAv9d__FE7pvWf3Tj0.png)



After (on click):

![img](images/TY4Qm-XG6EC56w6E9iNlChDEV5vCOhrEu7geq-gNU_6eBD4u7y-2ZdY21ZmWq9jgzkiU_LDrDqeCsog9teT45q2a0Qr8yhOANa6LTbEy9H99aiQOBSUmLxMpRx0q56EzaimRNMvJ.png)



