<script>
export default {
    props: {
        contacts: { type: Object, required: true },
    },
};
</script>

<template>
    <div>
        <div class="p-1">
            <strong>Tên:</strong>
            {{ contacts.name }}
        </div>
        <div class="p-1">
            <strong>E-mail:</strong>
            {{ contacts.email }}
        </div>
        <div class="p-1">
            <strong>Địa chỉ:</strong>
            {{ contacts.address }}
        </div>
        <div class="p-1">
            <strong>Điện thoại:</strong>
            {{ contacts.phone }}
        </div>
        <div class="p-1">
            <strong>Liên hệ yêu thích:&nbsp;</strong>
            <i v-if="contacts.favorite" class="fas fa-check"></i>
            <i v-else class="fas fa-times"></i>
        </div>
    </div>
</template>