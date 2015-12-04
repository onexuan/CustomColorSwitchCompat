# Change SwitchCompat color programmatically [CustomColorSwitchCompat]
Change color of SwitchCompat programmatically or in xml layout

## Programmatically
```
final CustomColorSwitchCompat switchRequestPin = (CustomColorSwitchCompat) findViewById(R.id.switchRequestPin);
switchRequestPin.setBgOnColor(Color.parseColor("#009284"));
switchRequestPin.setBgOffColor(Color.parseColor("#d0d0d0"));
switchRequestPin.setToggleOnColor(Color.parseColor("#97d9d7"));
switchRequestPin.setToggleOffColor(Color.parseColor("#a6a6a6"));
switchRequestPin.setOnCheckedChangeListener(new CompoundButton.OnCheckedChangeListener() {
    @Override
    public void onCheckedChanged(CompoundButton buttonView, boolean isChecked) {
        // TODO do something
    }
});
```

## XML Layout
```
<com.jahertor.customcolorswitchcompat.CustomColorSwitchCompat
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:id="@+id/switchRequestPin"
    android:layout_centerVertical="true"
    android:layout_alignParentRight="true"
    android:layout_alignParentEnd="true"
    android:layout_toRightOf="@id/hello"
    app:toggleOnColor="#009284"
    app:toggleOffColor="#d0d0d0"
    app:bgOnColor="#97d9d7"
    app:bgOffColor="#a6a6a6" />
```

## Getting started
Just import the code as a module in Android Studio.
