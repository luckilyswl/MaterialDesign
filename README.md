# MaterialDesign 、TopHover

1.Material Design 的布局
	
	<android.support.design.widget.CoordinatorLayout
		...>

		<android.support.design.widget.AppBarLayout
		...>

			<android.support.v7.widget.Toolbar
			.../>

		</android.support.design.widget.AppBarLayout>

		<android.support.v4.widget.SwipeRefreshLayout
		...>

		<android.support.v7.widget.RecyclerView
                .../>

        </android.support.v4.widget.SwipeRefreshLayout>

        <android.support.design.widget.FloatingActionButton
            .../>

	</android.support.design.widget.CoordinatorLayout>



2.TopHover 的布局框架

	<android.support.design.widget.CoordinatorLayout
         ...>

        <android.support.design.widget.AppBarLayout
            ...>

            <!--
            AppBarLayout里放入的都可以跟着向上滑动滑出布局的的，
            添加app:layout_scrollFlags="scroll"属性可以滑出布局
            TabLayout没有添加，所以停留在顶部
            -->

            <RelativeLayout
                ...>

                <!--头像-->
                <RelativeLayout
                    ...>

                    <ImageView
                        .../>

                    <!--<com.qingshangzuo.tophover.RoundImageView
                        android:id="@+id/userphotoCircleImageView"
                        android:layout_width="62dp"
                        android:layout_height="62dp"
                        android:layout_centerInParent="true"
                        android:scaleType="centerCrop"/>-->

                </RelativeLayout>

                <TextView
                   .../>

                <LinearLayout
                    ...>

                    <!--关注-->
                    <RelativeLayout
                        ...>

                        <TextView
                            .../>

                        <TextView
                            ... />

                    </RelativeLayout>

                    <!--粉丝-->
                    <RelativeLayout
                        android:id="@+id/followedsRelativeLayout"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_centerHorizontal="true"
                        android:layout_marginTop="16dp"
                        android:layout_marginLeft="18dp">

                        <TextView
                            ... />

                        <TextView
                            .../>

                    </RelativeLayout>

                </LinearLayout>

                <!--简介-->
                <TextView
                  .../>

            </RelativeLayout>

            <RelativeLayout
                ...>

                <View
                    .../>

                <TextView
                    .../>

                <LinearLayout
                    ...>

                    <LinearLayout
                        ...>

                        <TextView
                            .../>

                        <View
                            .../>

                    </LinearLayout>

                    <LinearLayout
                        ...>

                        <TextView
                            .../>

                        <View
                            .../>

                    </LinearLayout>

                    <LinearLayout
                        ...>

                        <TextView
                            .../>

                        <View
                            .../>

                    </LinearLayout>

                </LinearLayout>

                <!--<View
                    style="@style/mview"
                    android:id="@+id/view"
                    android:layout_below="@id/dynamicRelativeLayout"
                    android:layout_marginTop="2dp"/>-->

                <!--<TextView
                    android:id="@+id/hintTextView"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="此用户设置了隐藏个人动态信息"
                    android:textSize="16sp"
                    android:textColor="#E2E0DD"
                    android:layout_marginTop="15dp"
                    android:layout_centerHorizontal="true"
                    android:layout_below="@id/view"
                    android:visibility="gone"
                    />-->

            </RelativeLayout>

        </android.support.design.widget.AppBarLayout>

        <RelativeLayout
           ...>
            <android.support.v4.view.ViewPager
                ...>
            </android.support.v4.view.ViewPager>
        </RelativeLayout>

    </android.support.design.widget.CoordinatorLayout>

