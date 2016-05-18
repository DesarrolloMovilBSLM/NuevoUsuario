# NuevoUsuario
formulario


<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingTop="@dimen/activity_vertical_margin"
    tools:context="com.example.lupira.asflorvi.AgregarUsuario">

    <ScrollView
        android:layout_width="fill_parent"
        android:layout_height="fill_parent"
       >
    <LinearLayout
        android:layout_width="fill_parent"
        android:layout_height="fill_parent"
        android:orientation="vertical">


    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="@dimen/activity_horizontal_margin"
        android:layout_marginEnd="@dimen/activity_horizontal_margin"
        android:textAppearance="?android:attr/textAppearanceSmall"
        android:id="@+id/text_usuario"/>
    
    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:hint="Nombre de usuario"
        android:id="@+id/edit_nombre"
        android:layout_below="@+id/contrasena_usuario"
        android:layout_alignParentStart="true" />


    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/contrasena_usuario"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Constraseña" />

    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/ap_paterno"
        android:layout_below="@+id/edit_nombre"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Apellido paterno" />


        <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/ap_materno"
        android:layout_below="@+id/ap_paterno"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Apellido materno" />

    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/no_telefono"
        android:layout_below="@+id/ap_materno"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Número de teléfono" />

    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/correo"
        android:layout_below="@+id/no_telefono"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Correo" />


    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/calle"
        android:layout_below="@+id/correo"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Calle" />


    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/no_calle"
        android:layout_below="@+id/calle"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Número de calle" />

    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:id="@+id/comunidad"
        android:layout_below="@+id/no_calle"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Comunidad" />

    <EditText
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:inputType="number"
        android:id="@+id/no_socio"
        android:layout_below="@+id/comunidad"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:hint="Número de socio" />

        <EditText
            android:layout_width="match_parent"
            android:layout_height="50dp"
            android:inputType="number"
            android:id="@+id/nave"
            android:layout_below="@+id/no_socio"
            android:layout_alignParentStart="true"
            android:layout_alignParentEnd="true"
            android:hint="Nave" />

        <EditText
            android:layout_width="100dp"
            android:layout_height="50dp"
            android:inputType="number"
            android:id="@+id/noExtencion"
            android:layout_below="@+id/nave"
            android:hint="Extención de cultivo"
            android:layout_alignParentStart="true"
            android:layout_alignBottom="@+id/spinnerExtencion2"
            android:layout_toStartOf="@+id/spinnerExtencion2"
            android:layout_alignTop="@+id/spinnerExtencion2"
            />
        <Spinner
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:id="@+id/Variedades"
            android:layout_below="@id/nave"
            android:layout_alignParentEnd="true"
            android:layout_marginBottom="55dp"
            android:layout_alignStart="@+id/nave2"
            android:layout_toEndOf="@+id/noExtencion"
            />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textAppearance="?android:attr/textAppearanceLarge"
            android:text="  "
            android:id="@+id/textView"
            android:layout_below="@+id/Variedades"
            android:layout_alignParentStart="true" />

    </LinearLayout>
    </ScrollView>


    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:layout_alignParentBottom="true"
        android:orientation="horizontal"
        android:background="@color/colorPrimaryDark"
        style="?android:attr/buttonBarStyle">

        <Button
            android:id="@+id/bCancelarRegistros"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:textColor="@color/cardview_light_background"
            android:text="Cancelar"
            android:background="@color/colorPrimaryDark"/>

        <Button
            android:id="@+id/bAceptarRegistros"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:textColor="@color/cardview_light_background"
            android:text="Aceptar"
            android:background="@color/colorPrimaryDark" />

    </LinearLayout>

</RelativeLayout>




