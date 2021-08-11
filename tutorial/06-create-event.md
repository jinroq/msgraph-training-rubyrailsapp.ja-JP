<!-- markdownlint-disable MD002 MD041 -->

このセクションでは、ユーザーの予定表にイベントを作成する機能を追加します。

1. **./app/helpers/graph_helper.rb** を開き、次のメソッドをクラスに **Graph** します。

    :::code language="ruby" source="../demo/graph-tutorial/app/helpers/graph_helper.rb" id="CreateEventSnippet":::

1. **./app/controllers/calendar_controller** を開き **、CalendarController** クラスに次のルートを追加します。

    :::code language="ruby" source="../demo/graph-tutorial/app/controllers/calendar_controller.rb" id="CreateEventRouteSnippet":::

1. **./config/routes.rb を開き**、新しいルートを追加します。

    ```ruby
    post 'calendar/new', :to => 'calendar#create'
    ```

1. **./app/views/calendar/new.html.erb** を開き、その内容を次に置き換えます。

    :::code language="html" source="../demo/graph-tutorial/app/views/calendar/new.html.erb" id="NewEventFormSnippet":::

1. 変更を保存し、アプリを更新します。 [予定表 **] ページで** 、[新しいイベント] **ボタンを選択** します。 フォームに入力し、[作成] **を選択して** 新しいイベントを作成します。

    ![新しいイベント フォームのスクリーンショット](images/create-event-01.png)
