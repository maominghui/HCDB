//
//  AppDelegate.m
//  HCApp
//
//  Created by apple on 15/4/29.
//  Copyright (c) 2015年 wenkai. All rights reserved.
//

#import "AppDelegate.h"
#import "FirstViewController.h"
#import "SecondViewController.h"
#import "ThreeViewController.h"
#import "FourViewController.h"

@interface AppDelegate ()

@end

@implementation AppDelegate

#pragma mark - 增家TabBar控制器
- (void)addTabVC
{
    //添加UITabBarController
    self.window = [[UIWindow alloc] initWithFrame:[[UIScreen mainScreen] bounds]];
    self.window.backgroundColor = [UIColor whiteColor];
    
    //创建子控制器
    FirstViewController *firstVC = [[FirstViewController alloc] initWithNibName:@"FirstViewController" bundle:Nil];
    UINavigationController *firstNC = [[UINavigationController alloc] initWithRootViewController:firstVC];
    
    SecondViewController *secondVC = [[SecondViewController alloc] initWithNibName:@"SecondViewController" bundle:Nil];
    UINavigationController *secondNC = [[UINavigationController alloc] initWithRootViewController:secondVC];
    
    ThreeViewController *threeVC = [[ThreeViewController alloc] initWithNibName:@"ThreeViewController" bundle:Nil];
    UINavigationController *threeNC = [[UINavigationController alloc] initWithRootViewController:threeVC];
    
    FourViewController *fourVC = [[FourViewController alloc] initWithNibName:@"FourViewController" bundle:Nil];
    UINavigationController *fourNC = [[UINavigationController alloc] initWithRootViewController:fourVC];
    
    //初始化一个TabBar控制器
    UITabBarController *tb = [[UITabBarController alloc] init];
    
    tb.viewControllers = @[firstNC,secondNC,threeNC,fourNC];
    UITabBar *tabBar = tb.tabBar;
    
    UITabBarItem *aTabBarItem = [tabBar.items objectAtIndex:0];
    UITabBarItem *bTabBarItem = [tabBar.items objectAtIndex:1];
    UITabBarItem *cTabBarItem = [tabBar.items objectAtIndex:2];
    UITabBarItem *dTabBarItem = [tabBar.items objectAtIndex:3];
    
    //设置TabBar的图片和文字
    aTabBarItem.title = @"产品中心";
    aTabBarItem.image = [[UIImage imageNamed:@"产品中心"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    aTabBarItem.selectedImage = [[UIImage imageNamed:@"产品中心按下"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    
    bTabBarItem.title = @"活动专区";
    bTabBarItem.image = [[UIImage imageNamed:@"活动专区"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    bTabBarItem.selectedImage = [[UIImage imageNamed:@"活动专区按下"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    
    cTabBarItem.title = @"个人中心";
    cTabBarItem.image = [[UIImage imageNamed:@"个人中心"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    cTabBarItem.selectedImage = [[UIImage imageNamed:@"个人中心按下"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    
    dTabBarItem.title = @"更多";
    dTabBarItem.image = [[UIImage imageNamed:@"更多"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    dTabBarItem.selectedImage = [[UIImage imageNamed:@"更多按下"]  imageWithRenderingMode:UIImageRenderingModeAlwaysOriginal];
    [tabBar setTintColor:[UIColor yellowColor]];
    [tabBar setBackgroundImage:[UIImage imageNamed:@"底部背景"]];
    self.window.rootViewController = tb;
    //2.设置Window为主窗口并显示出来
    [self.window makeKeyAndVisible];
    
}
#pragma mark - 设置全局特性
- (void)setAppearanceFeature
{
    //在此处设置全局特性
}
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
    [self setAppearanceFeature];
    [self addTabVC];
  
    return YES;
}

- (void)applicationWillResignActive:(UIApplication *)application {
    // Sent when the application is about to move from active to inactive state. This can occur for certain types of temporary interruptions (such as an incoming phone call or SMS message) or when the user quits the application and it begins the transition to the background state.
    // Use this method to pause ongoing tasks, disable timers, and throttle down OpenGL ES frame rates. Games should use this method to pause the game.
}

- (void)applicationDidEnterBackground:(UIApplication *)application {
    // Use this method to release shared resources, save user data, invalidate timers, and store enough application state information to restore your application to its current state in case it is terminated later.
    // If your application supports background execution, this method is called instead of applicationWillTerminate: when the user quits.
}

- (void)applicationWillEnterForeground:(UIApplication *)application {
    // Called as part of the transition from the background to the inactive state; here you can undo many of the changes made on entering the background.
}

- (void)applicationDidBecomeActive:(UIApplication *)application {
    // Restart any tasks that were paused (or not yet started) while the application was inactive. If the application was previously in the background, optionally refresh the user interface.
}

- (void)applicationWillTerminate:(UIApplication *)application {
    // Called when the application is about to terminate. Save data if appropriate. See also applicationDidEnterBackground:.
}

@end
