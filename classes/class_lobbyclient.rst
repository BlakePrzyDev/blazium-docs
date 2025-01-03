:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/blazium-engine/blazium/tree/4.3/doc/tools/make_rst.py.
.. XML source: https://github.com/blazium-engine/blazium/tree/4.3/modules/blazium_sdk/doc_classes/LobbyClient.xml.

.. _class_LobbyClient:

LobbyClient
===========

**Inherits:** :ref:`BlaziumClient<class_BlaziumClient>`

**Inherited By:** :ref:`AuthoritativeClient<class_AuthoritativeClient>`

A node used to connect to a lobby server.

.. rst-class:: classref-introduction-group

Description
-----------

A node used to connect to a lobby server. It can be used to do matchmaking. You can do operations such as create lobby, join lobby, etc. The server is configurable and can either be self deployed or you can use the blazium free matchmaking server.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | ``bool``                                                       | :ref:`connected<class_LobbyClient_property_connected>`                   | ``false``                             |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | ``String``                                                     | :ref:`game_id<class_LobbyClient_property_game_id>`                       | ``""``                                |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | ``Dictionary``                                                 | :ref:`host_data<class_LobbyClient_property_host_data>`                   | ``{}``                                |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | :ref:`LobbyInfo<class_LobbyInfo>`                              | :ref:`lobby<class_LobbyClient_property_lobby>`                           |                                       |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | :ref:`LobbyPeer<class_LobbyPeer>`                              | :ref:`peer<class_LobbyClient_property_peer>`                             |                                       |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | ``Dictionary``                                                 | :ref:`peer_data<class_LobbyClient_property_peer_data>`                   | ``{}``                                |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | :ref:`Array<class_Array>`\[:ref:`LobbyPeer<class_LobbyPeer>`\] | :ref:`peers<class_LobbyClient_property_peers>`                           | ``[]``                                |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | ``String``                                                     | :ref:`reconnection_token<class_LobbyClient_property_reconnection_token>` | ``""``                                |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+
   | ``String``                                                     | :ref:`server_url<class_LobbyClient_property_server_url>`                 | ``"wss://lobby.blazium.app/connect"`` |
   +----------------------------------------------------------------+--------------------------------------------------------------------------+---------------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`add_lobby_data<class_LobbyClient_method_add_lobby_data>`\ (\ data\: ``Dictionary``, is_private\: ``bool`` = false\ )                                                  |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`add_lobby_tags<class_LobbyClient_method_add_lobby_tags>`\ (\ tags\: ``Dictionary``\ )                                                                                 |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`add_peer_data<class_LobbyClient_method_add_peer_data>`\ (\ data\: ``Dictionary``, target_peer\: ``String``, is_private\: ``bool`` = false\ )                          |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`add_peers_data<class_LobbyClient_method_add_peers_data>`\ (\ data\: ``Dictionary``, is_private\: ``bool`` = false\ )                                                  |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ``bool``                                          | :ref:`connect_to_lobby<class_LobbyClient_method_connect_to_lobby>`\ (\ )                                                                                                    |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`ViewLobbyResponse<class_ViewLobbyResponse>` | :ref:`create_lobby<class_LobbyClient_method_create_lobby>`\ (\ title\: ``String``, tags\: ``Dictionary`` = {}, max_players\: ``int`` = 4, password\: ``String`` = ""\ )     |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`del_lobby_data<class_LobbyClient_method_del_lobby_data>`\ (\ keys\: :ref:`Array<class_Array>`\[``String``\], is_private\: ``bool`` = false\ )                         |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`del_lobby_tags<class_LobbyClient_method_del_lobby_tags>`\ (\ keys\: :ref:`Array<class_Array>`\[``String``\]\ )                                                        |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`del_peer_data<class_LobbyClient_method_del_peer_data>`\ (\ keys\: :ref:`Array<class_Array>`\[``String``\], target_peer\: ``String``, is_private\: ``bool`` = false\ ) |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`del_peers_data<class_LobbyClient_method_del_peers_data>`\ (\ keys\: :ref:`Array<class_Array>`\[``String``\], is_private\: ``bool`` = false\ )                         |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`disconnect_from_lobby<class_LobbyClient_method_disconnect_from_lobby>`\ (\ )                                                                                          |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | ``bool``                                          | :ref:`is_host<class_LobbyClient_method_is_host>`\ (\ )                                                                                                                      |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`ViewLobbyResponse<class_ViewLobbyResponse>` | :ref:`join_lobby<class_LobbyClient_method_join_lobby>`\ (\ lobby_id\: ``String``, password\: ``String`` = ""\ )                                                             |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`kick_peer<class_LobbyClient_method_kick_peer>`\ (\ peer_id\: ``String``\ )                                                                                            |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`leave_lobby<class_LobbyClient_method_leave_lobby>`\ (\ )                                                                                                              |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`ListLobbyResponse<class_ListLobbyResponse>` | :ref:`list_lobbies<class_LobbyClient_method_list_lobbies>`\ (\ tags\: ``Dictionary`` = {}, start\: ``int`` = 0, count\: ``int`` = 10\ )                                     |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`notify_lobby<class_LobbyClient_method_notify_lobby>`\ (\ data\: ``Variant``\ )                                                                                        |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`notify_peer<class_LobbyClient_method_notify_peer>`\ (\ data\: ``Variant``, target_peer\: ``String``\ )                                                                |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`send_chat_message<class_LobbyClient_method_send_chat_message>`\ (\ chat_message\: ``String``\ )                                                                       |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`set_lobby_ready<class_LobbyClient_method_set_lobby_ready>`\ (\ ready\: ``bool``\ )                                                                                    |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`set_lobby_sealed<class_LobbyClient_method_set_lobby_sealed>`\ (\ seal\: ``bool``\ )                                                                                   |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LobbyResponse<class_LobbyResponse>`         | :ref:`set_peer_name<class_LobbyClient_method_set_peer_name>`\ (\ peer_name\: ``String``\ )                                                                                  |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`ViewLobbyResponse<class_ViewLobbyResponse>` | :ref:`view_lobby<class_LobbyClient_method_view_lobby>`\ (\ lobby_id\: ``String`` = "", password\: ``String`` = ""\ )                                                        |
   +---------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_LobbyClient_signal_connected_to_lobby:

.. rst-class:: classref-signal

**connected_to_lobby**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`, reconnection_token\: ``String``\ ) :ref:`🔗<class_LobbyClient_signal_connected_to_lobby>`

Signal generated after you connect to the lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_disconnected_from_lobby:

.. rst-class:: classref-signal

**disconnected_from_lobby**\ (\ reason\: ``String``\ ) :ref:`🔗<class_LobbyClient_signal_disconnected_from_lobby>`

Signal generated after you disconnect from the lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_lobby_created:

.. rst-class:: classref-signal

**lobby_created**\ (\ lobby\: :ref:`LobbyInfo<class_LobbyInfo>`, peers\: :ref:`Array<class_Array>`\[:ref:`LobbyPeer<class_LobbyPeer>`\]\ ) :ref:`🔗<class_LobbyClient_signal_lobby_created>`

Signal generated after a lobby is created.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_lobby_joined:

.. rst-class:: classref-signal

**lobby_joined**\ (\ lobby\: :ref:`LobbyInfo<class_LobbyInfo>`, peers\: :ref:`Array<class_Array>`\[:ref:`LobbyPeer<class_LobbyPeer>`\]\ ) :ref:`🔗<class_LobbyClient_signal_lobby_joined>`

Signal generated after you joint a lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_lobby_left:

.. rst-class:: classref-signal

**lobby_left**\ (\ kicked\: ``bool``\ ) :ref:`🔗<class_LobbyClient_signal_lobby_left>`

Signal generated after you leave a lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_lobby_notified:

.. rst-class:: classref-signal

**lobby_notified**\ (\ data\: ``Object``, from_peer\: :ref:`LobbyPeer<class_LobbyPeer>`\ ) :ref:`🔗<class_LobbyClient_signal_lobby_notified>`

Signal generated after a notification is received.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_lobby_sealed:

.. rst-class:: classref-signal

**lobby_sealed**\ (\ sealed\: ``bool``\ ) :ref:`🔗<class_LobbyClient_signal_lobby_sealed>`

Signal generated after the host seals the lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_lobby_tagged:

.. rst-class:: classref-signal

**lobby_tagged**\ (\ tags\: ``Dictionary``\ ) :ref:`🔗<class_LobbyClient_signal_lobby_tagged>`

Signal generated after the host updated the tags of the lobby

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_log_updated:

.. rst-class:: classref-signal

**log_updated**\ (\ command\: ``String``, logs\: ``String``\ ) :ref:`🔗<class_LobbyClient_signal_log_updated>`

Signals a log from a command.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_peer_disconnected:

.. rst-class:: classref-signal

**peer_disconnected**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`\ ) :ref:`🔗<class_LobbyClient_signal_peer_disconnected>`

Signal generated after a peer disconnects. If they don't reconnect they will be removed.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_peer_joined:

.. rst-class:: classref-signal

**peer_joined**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`\ ) :ref:`🔗<class_LobbyClient_signal_peer_joined>`

Signal generated after a peer joins the lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_peer_left:

.. rst-class:: classref-signal

**peer_left**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`, kicked\: ``bool``\ ) :ref:`🔗<class_LobbyClient_signal_peer_left>`

Signal generated after a peer leaves the lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_peer_messaged:

.. rst-class:: classref-signal

**peer_messaged**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`, chat_message\: ``String``\ ) :ref:`🔗<class_LobbyClient_signal_peer_messaged>`

Signal generated after a peer sends a chat message.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_peer_named:

.. rst-class:: classref-signal

**peer_named**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`\ ) :ref:`🔗<class_LobbyClient_signal_peer_named>`

Signal generated after a peer names himself.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_peer_ready:

.. rst-class:: classref-signal

**peer_ready**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`, is_ready\: ``bool``\ ) :ref:`🔗<class_LobbyClient_signal_peer_ready>`

Signal generated after a peer is ready.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_peer_reconnected:

.. rst-class:: classref-signal

**peer_reconnected**\ (\ peer\: :ref:`LobbyPeer<class_LobbyPeer>`\ ) :ref:`🔗<class_LobbyClient_signal_peer_reconnected>`

Signal generated after a peer reconnects.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_received_lobby_data:

.. rst-class:: classref-signal

**received_lobby_data**\ (\ data\: ``Object``, is_private\: ``bool``\ ) :ref:`🔗<class_LobbyClient_signal_received_lobby_data>`

Signal generated after data is sent to the lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_signal_received_peer_data:

.. rst-class:: classref-signal

**received_peer_data**\ (\ data\: ``Object``, to_peer\: :ref:`LobbyPeer<class_LobbyPeer>`, is_private\: ``bool``\ ) :ref:`🔗<class_LobbyClient_signal_received_peer_data>`

Signal generated after data is sent to peer.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_LobbyClient_property_connected:

.. rst-class:: classref-property

``bool`` **connected** = ``false`` :ref:`🔗<class_LobbyClient_property_connected>`

.. rst-class:: classref-property-setget

- ``bool`` **get_connected**\ (\ )

True if the client is connected, else false.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_game_id:

.. rst-class:: classref-property

``String`` **game_id** = ``""`` :ref:`🔗<class_LobbyClient_property_game_id>`

.. rst-class:: classref-property-setget

- |void| **set_game_id**\ (\ value\: ``String``\ )
- ``String`` **get_game_id**\ (\ )

The game id.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_host_data:

.. rst-class:: classref-property

``Dictionary`` **host_data** = ``{}`` :ref:`🔗<class_LobbyClient_property_host_data>`

.. rst-class:: classref-property-setget

- ``Dictionary`` **get_host_data**\ (\ )

The current lobby private data. Only works if you are host.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_lobby:

.. rst-class:: classref-property

:ref:`LobbyInfo<class_LobbyInfo>` **lobby** :ref:`🔗<class_LobbyClient_property_lobby>`

.. rst-class:: classref-property-setget

- :ref:`LobbyInfo<class_LobbyInfo>` **get_lobby**\ (\ )

The current lobby. Reflects changes to the lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_peer:

.. rst-class:: classref-property

:ref:`LobbyPeer<class_LobbyPeer>` **peer** :ref:`🔗<class_LobbyClient_property_peer>`

.. rst-class:: classref-property-setget

- :ref:`LobbyPeer<class_LobbyPeer>` **get_peer**\ (\ )

The current peer. Reflects changes to the self peer.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_peer_data:

.. rst-class:: classref-property

``Dictionary`` **peer_data** = ``{}`` :ref:`🔗<class_LobbyClient_property_peer_data>`

.. rst-class:: classref-property-setget

- ``Dictionary`` **get_peer_data**\ (\ )

The current peer private data.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_peers:

.. rst-class:: classref-property

:ref:`Array<class_Array>`\[:ref:`LobbyPeer<class_LobbyPeer>`\] **peers** = ``[]`` :ref:`🔗<class_LobbyClient_property_peers>`

.. rst-class:: classref-property-setget

- :ref:`Array<class_Array>`\[:ref:`LobbyPeer<class_LobbyPeer>`\] **get_peers**\ (\ )

The lobby peers. Reflects changes to all peers.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_reconnection_token:

.. rst-class:: classref-property

``String`` **reconnection_token** = ``""`` :ref:`🔗<class_LobbyClient_property_reconnection_token>`

.. rst-class:: classref-property-setget

- |void| **set_reconnection_token**\ (\ value\: ``String``\ )
- ``String`` **get_reconnection_token**\ (\ )

Reconnection token.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_property_server_url:

.. rst-class:: classref-property

``String`` **server_url** = ``"wss://lobby.blazium.app/connect"`` :ref:`🔗<class_LobbyClient_property_server_url>`

.. rst-class:: classref-property-setget

- |void| **set_server_url**\ (\ value\: ``String``\ )
- ``String`` **get_server_url**\ (\ )

Set to what url this lobby should connect to.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_LobbyClient_method_add_lobby_data:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **add_lobby_data**\ (\ data\: ``Dictionary``, is_private\: ``bool`` = false\ ) :ref:`🔗<class_LobbyClient_method_add_lobby_data>`

Add data to the lobby. Only works if you are host.

Generates :ref:`received_lobby_data<class_LobbyClient_signal_received_lobby_data>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_add_lobby_tags:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **add_lobby_tags**\ (\ tags\: ``Dictionary``\ ) :ref:`🔗<class_LobbyClient_method_add_lobby_tags>`

Add tags to the lobby. Only works if you are host.

Generates :ref:`lobby_tagged<class_LobbyClient_signal_lobby_tagged>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_add_peer_data:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **add_peer_data**\ (\ data\: ``Dictionary``, target_peer\: ``String``, is_private\: ``bool`` = false\ ) :ref:`🔗<class_LobbyClient_method_add_peer_data>`

Add data to a peer. Only works if you are host.

Generates :ref:`received_peer_data<class_LobbyClient_signal_received_peer_data>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_add_peers_data:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **add_peers_data**\ (\ data\: ``Dictionary``, is_private\: ``bool`` = false\ ) :ref:`🔗<class_LobbyClient_method_add_peers_data>`

Add data to all peers. Only works if you are host.

Generates :ref:`received_peer_data<class_LobbyClient_signal_received_peer_data>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_connect_to_lobby:

.. rst-class:: classref-method

``bool`` **connect_to_lobby**\ (\ ) :ref:`🔗<class_LobbyClient_method_connect_to_lobby>`

Connect to a Blazium Lobby Server using the :ref:`game_id<class_LobbyClient_property_game_id>` and :ref:`server_url<class_LobbyClient_property_server_url>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_create_lobby:

.. rst-class:: classref-method

:ref:`ViewLobbyResponse<class_ViewLobbyResponse>` **create_lobby**\ (\ title\: ``String``, tags\: ``Dictionary`` = {}, max_players\: ``int`` = 4, password\: ``String`` = ""\ ) :ref:`🔗<class_LobbyClient_method_create_lobby>`

Create a lobby and become host. If you are already in a lobby, you cannot create one. You need to leave first.

The new lobby can have a title, tags, max players and password. 0 max players means unlimited.

Generates :ref:`lobby_created<class_LobbyClient_signal_lobby_created>` signal.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_del_lobby_data:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **del_lobby_data**\ (\ keys\: :ref:`Array<class_Array>`\[``String``\], is_private\: ``bool`` = false\ ) :ref:`🔗<class_LobbyClient_method_del_lobby_data>`

Delete one or more keys from the lobby data. Only works if you are host.

Generates :ref:`received_lobby_data<class_LobbyClient_signal_received_lobby_data>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_del_lobby_tags:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **del_lobby_tags**\ (\ keys\: :ref:`Array<class_Array>`\[``String``\]\ ) :ref:`🔗<class_LobbyClient_method_del_lobby_tags>`

Delete one or more keys from the lobby tags. Only works if you are host.

Generates :ref:`lobby_tagged<class_LobbyClient_signal_lobby_tagged>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_del_peer_data:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **del_peer_data**\ (\ keys\: :ref:`Array<class_Array>`\[``String``\], target_peer\: ``String``, is_private\: ``bool`` = false\ ) :ref:`🔗<class_LobbyClient_method_del_peer_data>`

one or more keys from the peer data. Only works if you are host.

Generates :ref:`received_peer_data<class_LobbyClient_signal_received_peer_data>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_del_peers_data:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **del_peers_data**\ (\ keys\: :ref:`Array<class_Array>`\[``String``\], is_private\: ``bool`` = false\ ) :ref:`🔗<class_LobbyClient_method_del_peers_data>`

one or more keys from the peers data. Only works if you are host.

Generates :ref:`received_peer_data<class_LobbyClient_signal_received_peer_data>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_disconnect_from_lobby:

.. rst-class:: classref-method

|void| **disconnect_from_lobby**\ (\ ) :ref:`🔗<class_LobbyClient_method_disconnect_from_lobby>`

Disconnect from the lobby server.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_is_host:

.. rst-class:: classref-method

``bool`` **is_host**\ (\ ) :ref:`🔗<class_LobbyClient_method_is_host>`

Returns true if you are the host of the current lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_join_lobby:

.. rst-class:: classref-method

:ref:`ViewLobbyResponse<class_ViewLobbyResponse>` **join_lobby**\ (\ lobby_id\: ``String``, password\: ``String`` = ""\ ) :ref:`🔗<class_LobbyClient_method_join_lobby>`

Join a lobby. If you are already in a lobby, you cannot join another one. You need to leave first.

If the lobby you want to join is password protected, you need to provide the password.

Generates :ref:`lobby_joined<class_LobbyClient_signal_lobby_joined>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_kick_peer:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **kick_peer**\ (\ peer_id\: ``String``\ ) :ref:`🔗<class_LobbyClient_method_kick_peer>`

Kick a peer. You need to be host to do so.

Generates :ref:`peer_left<class_LobbyClient_signal_peer_left>` signal with kicked set to true.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_leave_lobby:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **leave_lobby**\ (\ ) :ref:`🔗<class_LobbyClient_method_leave_lobby>`

Leave a lobby. You need to be in a lobby to leave one.

Generates :ref:`lobby_left<class_LobbyClient_signal_lobby_left>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_list_lobbies:

.. rst-class:: classref-method

:ref:`ListLobbyResponse<class_ListLobbyResponse>` **list_lobbies**\ (\ tags\: ``Dictionary`` = {}, start\: ``int`` = 0, count\: ``int`` = 10\ ) :ref:`🔗<class_LobbyClient_method_list_lobbies>`

Lists all lobbies. Lobbies that are sealed won't show in the list, except if you disconnected and trying to reconnect to a lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_notify_lobby:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **notify_lobby**\ (\ data\: ``Variant``\ ) :ref:`🔗<class_LobbyClient_method_notify_lobby>`

Send a notification either to the host, or if you are host send data to all peers.

Generates :ref:`lobby_notified<class_LobbyClient_signal_lobby_notified>` signal.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_notify_peer:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **notify_peer**\ (\ data\: ``Variant``, target_peer\: ``String``\ ) :ref:`🔗<class_LobbyClient_method_notify_peer>`

Send a notification to a peer, works only if you are host.

Generates :ref:`lobby_notified<class_LobbyClient_signal_lobby_notified>` signal.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_send_chat_message:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **send_chat_message**\ (\ chat_message\: ``String``\ ) :ref:`🔗<class_LobbyClient_method_send_chat_message>`

Send a chat message. Only works if you are in a lobby.

Generates :ref:`peer_messaged<class_LobbyClient_signal_peer_messaged>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_set_lobby_ready:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **set_lobby_ready**\ (\ ready\: ``bool``\ ) :ref:`🔗<class_LobbyClient_method_set_lobby_ready>`

Ready up in the lobby. You need to be in a lobby and unready to run this.

Generates :ref:`peer_ready<class_LobbyClient_signal_peer_ready>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_set_lobby_sealed:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **set_lobby_sealed**\ (\ seal\: ``bool``\ ) :ref:`🔗<class_LobbyClient_method_set_lobby_sealed>`

Seals the lobby. You need to be the host to do this and the lobby needs to be unsealed.

Generates :ref:`lobby_sealed<class_LobbyClient_signal_lobby_sealed>`.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_set_peer_name:

.. rst-class:: classref-method

:ref:`LobbyResponse<class_LobbyResponse>` **set_peer_name**\ (\ peer_name\: ``String``\ ) :ref:`🔗<class_LobbyClient_method_set_peer_name>`

Set your peer name.

Generates :ref:`peer_named<class_LobbyClient_signal_peer_named>` signal if you are in lobby.

.. rst-class:: classref-item-separator

----

.. _class_LobbyClient_method_view_lobby:

.. rst-class:: classref-method

:ref:`ViewLobbyResponse<class_ViewLobbyResponse>` **view_lobby**\ (\ lobby_id\: ``String`` = "", password\: ``String`` = ""\ ) :ref:`🔗<class_LobbyClient_method_view_lobby>`

View data from a lobby. Returns lobby settings and peers.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
