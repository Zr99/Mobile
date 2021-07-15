1.
A Fragment represents a behavior or a portion of user interface in a FragmentActivity.
You can combine multiple fragments in a single activity to build a multi-pane UI and reuse a
fragment in multiple activities. You can think of a fragment as a modular section of an activity,
which has its own lifecycle, receives its own input events, and which you can add or remove while
the activity is running (sort of like a "sub activity" that you can reuse in different activities).

A fragment must always be hosted in an activity and the fragment's lifecycle is directly affected
by the host activity's lifecycle. For example, when the activity is paused, so are all fragments
in it, and when the activity is destroyed, so are all fragments. However, while an activity is
running (it is in the resumed lifecycle state), you can manipulate each fragment independently,
such as add or remove them. When you perform such a fragment transaction, you can also add it to a
back stack that's managed by the activity—each back stack entry in the activity is a record of the
fragment transaction that occurred. The back stack allows the user to reverse a fragment
transaction (navigate backwards), by pressing the Back button.

When you add a fragment as a part of your activity layout, it lives in a ViewGroup inside the
activity's view hierarchy and the fragment defines its own view layout. You can insert a fragment
into your activity layout by declaring the fragment in the activity's layout file, as a <fragment>
 element, or from your application code by adding it to an existing ViewGroup.

 2.

 I will leave the layout component as normal and keep the rest of the view group into a xml file.
 Then, refer back the xml file to the linear layout or constraint layout that I want to the specific
 xml file. The benefit of using fragment is to reduce the repeating codes that would have in both
 of the activity_main.xml files. Not only reduce the size of the application, it will also reduce
 the debugging errors that might occurs.
