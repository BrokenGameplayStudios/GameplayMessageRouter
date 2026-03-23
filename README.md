# Gameplay Message Router

A powerful decoupled messaging system originally from Epic's Lyra Starter Game for Unreal Engine 5.

Send and receive messages between completely unconnected gameplay objects using Gameplay Tags. No hard references needed.

## Features

* Publisher/Subscriber system using Gameplay Tags as channels
* Support for custom message payloads (any struct)
* Fully decoupled communication between systems
* Blueprint and C++ support
* Includes K2 nodes for easy Blueprint usage
* Local-player scoped (great companion to Gameplay Events)
* 100% multiplayer ready
* No dependencies

## Installation

1) Create folder `Plugins/GameplayMessageRouter` in your project
2) Copy the plugin files from this repo into it
3) Enable the plugin in the Editor
4) Restart Editor

## Quick Start

1) Get the Gameplay Message Subsystem (available in GameInstance or PlayerState)
2) Register listeners: `RegisterListener(GameplayTag, Callback)`
3) Broadcast messages: `BroadcastMessage(GameplayTag, PayloadStruct)`

Perfect for UI updates, cross-system events, achievements, inventory, and more without tight coupling.

## About

Standalone version of Epic Games' Gameplay Message Router from Lyra. Maintained by Broken Gameplay Studios.
