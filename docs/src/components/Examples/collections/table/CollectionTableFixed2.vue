<template>
  <div>
    <div class="ui ignored info message">
      Fixed <code>single line</code> tables will automatically ensure content that does not fit in a single line will receive "..." ellipsis
    </div>
    <table class="ui fixed single line celled table">
      <thead>
        <th>Name</th>
        <th>Status</th>
        <th>Description</th>
      </thead>
      <tbody>
        <tr>
          <td>John</td>
          <td>Approved</td>
          <td title="This is much too long to fit I'm sorry about that">This is much too long to fit I'm sorry about that</td>
        </tr>
        <tr>
          <td>Jamie</td>
          <td>Approved</td>
          <td>Shorter description</td>
        </tr>
        <tr>
          <td>Jill</td>
          <td>Denied</td>
          <td>Shorter description</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'CollectionTableFixed2',
  info: {
    converted: false,
    elementType: 'collections',
    element: 'table',
    title1: 'Variations',
    title2: 'Fixed',
    description: 'A table can use',
    model: '    <div class="ui ignored info message">\n' +
      '      Fixed <code>single line</code> tables will automatically ensure content that does not fit in a single line will receive "..." ellipsis\n' +
      '    </div>\n' +
      '    <table class="ui fixed single line celled table">\n' +
      '      <thead>\n' +
      '        <th>Name</th>\n' +
      '        <th>Status</th>\n' +
      '        <th>Description</th>\n' +
      '      </thead>\n' +
      '      <tbody>\n' +
      '        <tr>\n' +
      '          <td>John</td>\n' +
      '          <td>Approved</td>\n' +
      '          <td title="This is much too long to fit I\'m sorry about that">This is much too long to fit I\'m sorry about that</td>\n' +
      '        </tr>\n' +
      '        <tr>\n' +
      '          <td>Jamie</td>\n' +
      '          <td>Approved</td>\n' +
      '          <td>Shorter description</td>\n' +
      '        </tr>\n' +
      '        <tr>\n' +
      '          <td>Jill</td>\n' +
      '          <td>Denied</td>\n' +
      '          <td>Shorter description</td>\n' +
      '        </tr>\n' +
      '      </tbody>\n' +
      '    </table>\n',
  },
};
</script>
