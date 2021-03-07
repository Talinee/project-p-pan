<template>
  <a-table :columns="columns" :data-source="data">
    <a slot="name" slot-scope="text">{{ text }}</a>
  </a-table>
</template>
<script>
const columns = [
  {
    title: 'ผู้ใช้',
    dataIndex: 'Username',
    key: 'Username',
    scopedSlots: { customRender: 'Username' },
  },
    {
    title: 'สถานะ',
    dataIndex: 'type',
    key: 'type',
    scopedSlots: { customRender: 'type' },
  },
  {
    title: 'สถานที่',
    dataIndex: 'location',
    key: 'location',
  },
  {
    title: 'วันเวลา',
    dataIndex: 'date',
    key: 'date',
    ellipsis: true,
  },
  {
    title: 'อุณหภูมิ',
    dataIndex: 'temp',
    key: 'temp',
    ellipsis: true,
  },
];

const data = [
  {
    key: '1',
    Username: 'J',
    type: 'เข้า',
    location: 'ประตูภาควิชาวิศวกรรมไฟฟ้า คณะวิศวกรรมศาสตร์',
    date: '5 มีนาคม 2564 12:00 น.',
    temp: 36.5,
  },
  {
    key: '2',
    Username: 'Fram',
    type: 'เข้า',
    location: 'ประตูภาควิชาวิศวกรรมไฟฟ้า คณะวิศวกรรมศาสตร์',
    date: '5 มีนาคม 2564 12:10 น.',
    temp: 36.7,
  },
  {
    key: '3',
    Username: 'J',
    type: 'ออก',
    location: 'ประตูภาควิชาวิศวกรรมไฟฟ้า คณะวิศวกรรมศาสตร์',
    date: '5 มีนาคม 2564 12:30 น.',
    temp: null,
  },
  {
    key: '4',
    Username: 'J',
    type: 'เข้า',
    location: 'ประตูภาควิชาวิศวกรรมไฟฟ้า คณะวิศวกรรมศาสตร์',
    date: '5 มีนาคม 2564 12:40 น.',
    temp: 37,
  },
  {
    key: '5',
    Username: 'J',
    type: 'ออก',
    location: 'ประตูภาควิชาวิศวกรรมไฟฟ้า คณะวิศวกรรมศาสตร์',
    date: '5 มีนาคม 2564 13:00 น.',
    temp: null,
  },
  {
    key: '6',
    Username: 'Fram',
    type: 'ออก',
    location: 'ประตูภาควิชาวิศวกรรมไฟฟ้า คณะวิศวกรรมศาสตร์',
    date: '5 มีนาคม 2564 14:00 น.',
    temp: null,
  },
  {
    key: 'ึ',
    Username: 'Fram',
    type: 'ออก',
    location: 'ประตูภาควิชาวิศวกรรมไฟฟ้า คณะวิศวกรรมศาสตร์',
    date: '5 มีนาคม 2564 14:10 น.',
    temp: 37,
  },
];

export default {
  data() {
    return {
      data,
      columns,
    };
  },
};
</script>
