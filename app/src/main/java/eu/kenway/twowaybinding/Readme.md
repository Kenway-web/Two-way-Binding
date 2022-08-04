<TextView android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:text="@{myViewModel.username}"----------------->
android:textSize="40sp"
app:layout_constraintBottom_toBottomOf="parent"
app:layout_constraintLeft_toLeftOf="parent"
app:layout_constraintRight_toRightOf="parent"
app:layout_constraintTop_toTopOf="parent" />

<EditText android:id="@+id/editTextTextPersonName"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:ems="10"
android:inputType="textPersonName"
android:textSize="40sp"
android:text="@={myViewModel.username}"   ------------------>
app:layout_constraintBottom_toBottomOf="parent"
app:layout_constraintEnd_toEndOf="parent"
app:layout_constraintHorizontal_bias="0.5"
app:layout_constraintStart_toStartOf="parent"
app:layout_constraintTop_toTopOf="parent"
app:layout_constraintVertical_bias="0.26" />


look at the arrow part of both the section of code and observe the difference  .
Got something?
--
--
--
see the EditText   text attribute as "="  between @{   thats what doing two way binding.
--
If you remove '=', then there will be only one way binding
