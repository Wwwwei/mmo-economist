<!--
 * @Author: Shiwei Zhao
 * @Date: 2023-08-18 10:10:33
 * @FilePath: \mmo-economist\README.md
 * Copyright (c) 2023 by NetEase, Inc., All Rights Reserved.
-->
# the-MMO-Economist
This repo is the unofficial implementation of The MMO Economist. 
The MMO Economist is an economic simulation environment that facilitates the correspondence between real-world economic systems and their virtual counterparts for authentic and realistic assessments of MMO (Massively Multiplayer Online Game) economic evolution.

## Requirements
The code has been tested running under Python 3.8.16, with the following packages installed (along with their dependencies):
- gym==0.21
- tensorflow==1.14
- ray[rllib]==0.8.4
- importlib-metadata==4.13.0

## Components
- Economic Resource
  - **EXP**: Non-negotiable incorporeal game assets, acquired directly from the game and used solely by the player oneself, without trading possibilities.
  - **MAT**: Negotiable corporeal game assets, directly obtained from the game and tradable with others.
  - **TOK**: Any item that can function as a general equivalent to all goods and services in games, obtained directly from the game or through external recharges.
  - **CCY**: Legal tender of a specific country used externally to the game, utilized for recharges to exchange for tokens.
  - **CAP**: Specific (virtual) abilities or scores that players enhance by participating in various game activities.
  - **LAB**: Labor generated by players engaging in game activities during the game.
- Economic Activity
  - **Task**: Any production behavior in which players directly obtain resources through their labor in the game.
  - **Upgrade**: Any consuming behavior of players to improve their capabilities by consuming corresponding economic resources in the game.
  - **Auction**: Any trade behavior involving free trade between players in the game. All tradable economic resources can be traded structured as a continuous double auction.
  - **Shop**: Any trade behavior where players directly purchase commodities from game malls or non-player characters~(NPCs) in the game.
  - **Recharge**: Any forex behavior where players make payments in the game, such as IAP.
- Economic Entity: **Agent players with different personalities.**
- Economic Structure
  - **Market Economy**: Free economy without any economic regulation and control
  - **Planned Economy**: Economy with economic regulation and control by human or AI 

## Running
- demo.ipynb: This demo shows how environmen works in economic simulations.
- demo_rllib_yaml.ipynb: This demo shows how AI works in economic design.

## Acknowledgements
We thank the great work [the ai economist](https://github.com/salesforce/ai-economist/tree/master) for providing assistance for our research.
