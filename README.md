实验目的
---
练习对LinearLayout,ConstrainLayout,TableLayout的使用。<br>
关键代码
--
1.LinearLayout
  文件名：activity_main.xml
'''
<?xml version="1.0" encoding="utf-8"?>

<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:orientation="horizontal">

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn11" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="4"
            android:text="@string/btn12" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn13" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn14" />
    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:orientation="horizontal">

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn21" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="4"
            android:text="@string/btn22" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn23" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn24" />
    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:orientation="horizontal">

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn31" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn32" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn33" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn34" />
    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:orientation="horizontal">

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn41" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="4"
            android:text="@string/btn42" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn43" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:text="@string/btn44" />
    </LinearLayout>

</LinearLayout>
'''
2.ConstrainLayout
  文件名：activity_main2.xml
'''
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:id="@+id/textView3"
        android:layout_width="80dp"
        android:layout_height="80dp"
        android:background="@color/red"
        android:fontFamily="serif"
        android:gravity="center"
        android:text="RED"
        android:textAlignment="center"
        android:textAllCaps="false"
        android:textAppearance="@android:style/TextAppearance.Large"
        android:textColor="@android:color/black"
        android:textSize="18sp"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="110dp"
        android:layout_height="80dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:background="@color/orange"
        android:gravity="center"
        android:text="ORANGE"
        android:textSize="18sp"
        android:textStyle="bold"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/YELLOW"
        android:layout_width="110dp"
        android:layout_height="80dp"
        android:background="@color/yellow"
        android:gravity="center"
        android:text="TextView"
        android:textSize="18sp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView6"
        android:layout_width="80dp"
        android:layout_height="62dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/green"
        android:gravity="center"
        android:text="GREEN"
        android:textSize="18sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.3"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView7"
        android:layout_width="80dp"
        android:layout_height="62dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/blue"
        android:gravity="center"
        android:text="BLUE"
        android:textColor="@android:color/white"
        android:textSize="18sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.503" />

    <TextView
        android:id="@+id/textView8"
        android:layout_width="80dp"
        android:layout_height="62dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/indigo"
        android:gravity="center"
        android:text="INDIGO"
        android:textColor="@android:color/white"
        android:textSize="18sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.7"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.497" />

    <TextView
        android:id="@+id/VIOLET"
        android:layout_width="0dp"
        android:layout_height="60dp"
        android:background="@color/violet"
        android:gravity="center"
        android:text="VIOLET"
        android:textSize="18sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="1.0" />

</android.support.constraint.ConstraintLayout>
'''
3.TableLayout
  文件名：activity_main3.xml
'''
<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:stretchColumns="1"
    android:shrinkColumns="0,2">
    <TableRow>

        <TextView
            android:text="    Open..."
            android:textSize="18sp" />
        <TextView />
        <TextView
            android:text="Ctrl-O"
            android:gravity="right"
            android:textSize="18sp"/>
    </TableRow>

    <TableRow>

        <TextView
            android:text="    Save..."
            android:textSize="18sp" />
        <TextView />
        <TextView
            android:text="Ctrl-S"
            android:gravity="right"
            android:textSize="18sp"/>
    </TableRow>

    <TableRow>

        <TextView
            android:text="    Save As..."
            android:textSize="18sp" />
        <TextView />
        <TextView
            android:text="Ctrl-Shift-S"
            android:gravity="right"
            android:textSize="18sp"/>
    </TableRow>

    <TextView
        android:layout_height="1dp"
        android:layout_width="match_parent"
        android:background="#000000"/>

    <TableRow>
        <TextView
            android:text="X Import..."
            android:textSize="18sp" />
        <TextView />
    </TableRow>

    <TableRow>
        <TextView
            android:text="X Export..."
            android:textSize="18sp" />
        <TextView />
        <TextView
            android:text="Ctrl-E"
            android:gravity="right"
            android:textSize="18sp"/>
    </TableRow>

    <TextView
        android:layout_height="1dp"
        android:layout_width="match_parent"
        android:background="#000000"/>

    <TableRow>
        <TextView
            android:text="    Quit"
            android:textSize="18sp" />
        <TextView />
    </TableRow>



</TableLayout>
'''
结果截图
---
1.<br>
![image]()
